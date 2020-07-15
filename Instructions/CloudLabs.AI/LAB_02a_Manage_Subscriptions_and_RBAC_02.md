### Clean up resources

   >**Note**: Remember to remove any newly created Azure resources that you no longer use. 

   >**Note**: Removing unused resources ensures you will not see unexpected charges, although, resources created in this lab do not incur extra cost.

1. In the Azure portal, search for and select **Azure Active Directory**, on the Azure Active Directory blade, click **Users**.

1. On the **Users - All users** blade, click **az104-02-aaduser1**.

1. On the **az104-02-aaduser1 - Profile** blade, copy the value of **Object ID** attribute.

1. In the Azure portal, start a **PowerShell** session within the **Cloud Shell**.

1. From the Cloud Shell pane, run the following to remove the assignment of the custom role definition (replace the `[object_ID]` placeholder with the value of the **object ID** attribute of the **az104-02-aaduser1** Azure Active Directory user account you copied earlier in this task):

   ```pwsh
   $scope = (Get-AzRoleAssignment -RoleDefinitionName 'Support Request Contributor (Custom)').Scope

   Remove-AzRoleAssignment -ObjectId '[object_ID]' -RoleDefinitionName 'Support Request Contributor (Custom)' -Scope $scope
   ```

1. From the Cloud Shell pane, run the following to remove the custom role definition:

   ```pwsh
   Remove-AzRoleDefinition -Name 'Support Request Contributor (Custom)' -Force
   ```

1. In the Azure portal, navigate back to the **Users - All users** blade of the **Azure Active Directory**, and delete the **az104-02-aaduser1** user account.

1. In the Azure portal, navigate to the **az104-02-mg1** management group and display its **details**.

1. Right-click the **ellipsis** icon to the right of the entry representing your Azure subscription and click **Move**.

1. On the **Move** blade, select the management group which the subscription was originally part of and click **Save**. 

1. Navigate back to the **Management groups** blade, right click the **ellipsis** icon to the right of the **az104-02-mg1** management group and click **Delete**.

