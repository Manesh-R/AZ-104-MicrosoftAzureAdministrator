### Clean up resources

   >**Note**: Remember to remove any newly created Azure resources that you no longer use. Removing unused resources ensures you will not incur unexpected costs. While, in this case, there are no additional charges associated with Azure Active Directory tenants and their objects, you might want to consider removing the user accounts, the group accounts, and the Azure Active Directory tenant you created in this lab.

1. Navigate to the **Azure Active Directory Premium P2 - Licensed users** blade, select the user accounts to which you assigned licenses in this lab, click **Remove license**, and, when prompted to confirm, click **OK**.

1. In the Azure portal, navigate to the **Users - All users** blade, click the entry representing the **az104-01b-aaduser1** guest user account, on the **az104-01b-aaduser1 - Profile** blade click **Delete**, and, when prompted to confirm, click **OK**.

1. Repeat the same sequence of steps to delete the remaining user accounts you created in this lab.

1. Navigate to the **Groups - All groups** blade, select the groups you created in this lab, click **Delete**, and, when prompted to confirm, click **OK**.

1. In the Azure portal, display the blade of the Contoso Lab Azure AD tenant by using the **Directory + Subscription** button (directly to the right of the Cloud Shell button) in the Azure portal toolbar.

1. Navigate to the **Users - All users** blade, click the entry representing the **az104-01b-aaduser1** user account, on the **az104-01b-aaduser1 - Profile** blade click **Delete**, and, when prompted to confirm, click **OK**.

1. Navigate to the **Contoso Lab - Overview** blade of the Contoso Lab Azure AD tenant, click **Delete tenant**, on the **Delete directory 'Contoso Lab'** blade, click the **Get permission to delete Azure resources** link, on the **Properties** blade of Azure Active Directory, set **Access management for Azure resources** to **Yes** and click **Save**.

1. Sign out from the Azure portal and sign in back. 

1. Navigate back to the **Delete directory 'Contoso Lab'** blade and click **Delete**.

