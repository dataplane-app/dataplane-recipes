# Sharepoint API

Before using the Sharepoint API, an Azure App needs to be created. If you haven't done so already, follow these instructions. [register-an-azure-app.md](register-an-azure-app.md "mention")



**Assign Sharepoint API permissions to your Azure App**

a. Select API permissions

b. Add a permission

c. Find Sharepoint

d. Select Application Permissions - this allows a server side application to interact with the Sharepoint API.&#x20;

![](<../.gitbook/assets/image (4) (1).png>)

**Select permissions that is needed**

* Sites.FullControl.All - allows the creation of a Sharepoint site
* Sites.ReadWrite.All - allows reading and writing files to a Sharepoint site.

![](<../.gitbook/assets/image (3) (1).png>)

{% embed url="https://gist.github.com/feabced59a82e45859f3da3db463c222.git" %}
