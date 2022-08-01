# Register an Azure app

To interact with Office 365 APIs, you need to register an Azure app in Azure Portal. Once an app is created, assign specific API permissions that you need.&#x20;

1. Login at [https://portal.azure.com](https://portal.azure.com)
2. Go to App registrations&#x20;

![](<../.gitbook/assets/image (5).png>)

3\. Create an app

![](<../.gitbook/assets/image (1).png>)

4\. Create a secret

{% hint style="danger" %}
It is important to keep these credentials safe using a key store. It is good security practice not to hard code the secret in your code. Do not share secrets as this will compromise the safety and security of your data. You can use Dataplane's secrets to store these credentials. Learn more here: [https://learn.dataplane.app/managing-secrets](https://learn.dataplane.app/managing-secrets)
{% endhint %}

a. Click on Certificates & secrets

b. Click on New client secret

c. Store the value and secret ID in your Key Management System

![](<../.gitbook/assets/image (2) (1).png>)

5\. Add secrets to Dataplane

{% hint style="info" %}
The environment variables shown in the images below will be used to safely to retrieve the secrets inside the pipelines.
{% endhint %}



These variables will be used to authenticate with the Microsoft Graph API

* Add the Secret ID  - Environment variable: <mark style="color:purple;">secret\_</mark>_<mark style="color:purple;">dp</mark>_<mark style="color:purple;">\_office\_</mark>_<mark style="color:purple;">365\_</mark>_<mark style="color:purple;">id</mark>
* Add the Secret   - Environment variable: <mark style="color:purple;">secret\_</mark>_<mark style="color:purple;">dp</mark>_<mark style="color:purple;">\_office\_</mark>_<mark style="color:purple;">365\_secret</mark>_
* Tenant ID - Environment variable: <mark style="color:purple;">secret\_</mark>_<mark style="color:purple;">dp</mark>_<mark style="color:purple;">\_office\_</mark>_<mark style="color:purple;">365\_tenant\_id</mark>_

![](../.gitbook/assets/image.png)

![](<../.gitbook/assets/image (6).png>)

**Get the Tenant ID from your app**

a. Click on Overview

b. Get the Directory (Tenant) ID&#x20;

![](<../.gitbook/assets/image (2).png>)

c. Add Directory (Tenant) ID into Dataplane secrets

![](<../.gitbook/assets/image (4).png>)

