## Getting Started:


###### Description
 
This action pack integrates with the popular Office365 suite. It provides an outbound integration of the Automation Engine into your Office365 environment. This action pack enables you to carry out administrative tasks around your Office365 such as creating/deleting mailboxes and creating/deleting/updating groups.

###### Actions
 
 1.  Add Members to Group
 2.  Add Permissions to a Mailbox
 3.  Create Group
 4.  Create Mailbox
 5.  Create Shared Mailbox
 6.  Delete Group
 7.  Delete MailBox
 8.  Delete Members from the Group
 9.  Remove Permissions in a Mailbox
 10. Update Group
 11. Update Mailbox
  
 ###### Compatibility:

1. Oracle Java 1.8 or later
2. Microsoft Powershell 4 
3. Microsoft Support Exchange Online 

###### Prerequisite:

1. Automation Engine should be installed.
2. Automic Package Manager should be installed.
3. ITPA Shared Action Pack should be installed. 
4. Maven

###### To create an account on Microsoft 365 Admin Center
The Microsoft Office 365 Admin Center is the web portal from which each company's service administrator can manage user accounts and settings for each of the Office 365.

Create an account by registering to Microsoft 365 Admin Center, URL: https://www.microsoft.com/en-in/microsoft-365/business/office-365-administration

###### Steps to install action pack source code:

1. Clone the code to your machine.
2. Go to the package directory.
3. Run the maven command 'mvn clean package' inside the directory containing the pom.xml file.(source/tools/)
4. Run the command apm upload in the directory which contains package.yml (source/):
   Ex. apm upload -force -u <Name>/<Department> -c <Client-id> -H <Host> -pw <Password> -S AUTOMIC -y -ia -ru


###### Package/Action Documentation

Please refer to the link for [package documentation](source/ae/content/DOCUMENTATION/PCK.AUTOMIC_MICROSOFT_OFFICE365.PUB.DOC.xml)

###### Third party licenses:

The third-party library and license document reference.[Third party licenses](source/ae/content/DOCUMENTATION/PCK.AUTOMIC_MICROSOFT_OFFICE365.PUB.LICENSES.xml)

###### Useful References

1. [About Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_AboutPacksandPlugins.htm?Highlight=Action%20packs)
2. [Working with Packs and Plug-ins](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#PluginManager/PM_WorkingWith.htm#link10)
3. [Actions and Action Packs](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#_Common/ReleaseHighlights/RH_Plugin_PackageManager.htm?Highlight=Action%20packs)
4. [PACKS Compatibility Mode](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#AWA/Variables/UC_CLIENT_SETTINGS/UC_CLIENT_PACKS_COMPATIBILITY_MODE.htm?Highlight=Action%20packs)
5. [Working with actions](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/AB_WorkingWith.htm#link4)
6. [Installing and Configuring the Action Builder](https://docs.automic.com/documentation/webhelp/english/AA/12.3/DOCU/12.3/Automic%20Automation%20Guides/help.htm#ActionBuilder/install_configure_plugins_AB.htm?Highlight=Action%20packs)

###### Distribution: 

In the distribution process, we can download the existing or updated action package from the Automation Engine by using the apm build command.
Example: **apm build -y -H AE_HOST -c 106 -u TEST/TEST -pw password -d /directory/ -o zip -v action_pack_name**
			
			
###### Copyright and License: 

Broadcom does not support, maintain or warrant Solutions, Templates, Actions and any other content published on the Community and is subject to Broadcom Community [Terms and Conditions](https://community.broadcom.com/termsandconditions)

 