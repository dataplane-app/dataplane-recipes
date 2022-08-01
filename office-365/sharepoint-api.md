# Sharepoint API

### Before using the Sharepoint API

* An Azure App needs to be created. If you haven't done so already, follow these instructions. [register-an-azure-app.md](register-an-azure-app.md "mention")
* Assign Sharepoint permissions - see below for instructions
* To use Rest APIs, install the requests pip package by adding `requests==2.28.1` to requirements.txt file. Instructions: [https://learn.dataplane.app/create-a-data-pipeline#update-python-packages](https://learn.dataplane.app/create-a-data-pipeline#update-python-packages)

### **Assign Sharepoint API permissions to your Azure App**

a. Select API permissions

b. Add a permission

c. Find Sharepoint

d. Select Application Permissions - this allows a server side application to interact with the Sharepoint API.&#x20;

![](<../.gitbook/assets/image (4) (1).png>)

**Select permissions that is needed**

* Sites.FullControl.All - allows the creation of a Sharepoint site
* Sites.ReadWrite.All - allows reading and writing files to a Sharepoint site.

![](<../.gitbook/assets/image (3) (1).png>)

### Run the APIs in Dataplane's code editor

To use Dataplane's code editor, see [https://learn.dataplane.app/create-a-data-pipeline#write-and-test-python-code](https://learn.dataplane.app/create-a-data-pipeline#write-and-test-python-code)

{% embed url="https://gist.github.com/feabced59a82e45859f3da3db463c222.git" %}
