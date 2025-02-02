# How to deploy an Aspire .NET 9 application with Azure Developers CLI (azd)

## 1. Install Azure Developer CLI

See the detailed information in this URL:

https://learn.microsoft.com/es-es/azure/developer/azure-developer-cli/install-azd

We run this command to install Azure Developer CLI (azd)

```
choco install azd
```

![image](https://github.com/user-attachments/assets/6b73786f-45b3-47ac-b471-47b461319b6d)

We verify the azd installation

```
azd version
```

![image](https://github.com/user-attachments/assets/aa03eec7-8c2e-4701-8ac9-70ba42ea8163)

## 2. We create the application with Visual Studio 2022 Community Edition and .NET 9



## 3. We run the azd commands

We have to right click on the Solution name and select the menu option **Open Folder in File Explorer**

![image](https://github.com/user-attachments/assets/529962f1-a57d-47cc-9a71-ec88cfe4a2c6)

![image](https://github.com/user-attachments/assets/fd817677-f95f-47a9-8f92-960f17f5abb5)

Now we can run the **cmd** to open the command prompt for running the **azd** commands

![image](https://github.com/user-attachments/assets/dc8e4237-d605-4a61-9c7d-20c877fb6496)

### 3.1. Initialize an Application (azd init)

This initializes a new Azure Developer environment. You can choose a template or provide an existing project

It helps set up the structure for your application, including the necessary configuration files

```
azd init
```

![image](https://github.com/user-attachments/assets/a01143c3-cb8d-46ed-b3f7-5f235dcccc6d)

### 3.2. Azure login

```
azd auth login
```

![image](https://github.com/user-attachments/assets/41107dd2-f0ed-4282-b7a6-8e9ff36ab104)

### 3.3. Provision Resources (azd provision):

```
azd provision
```

This command creates all the Azure resources defined for your application, such as App Services, databases, and storage accounts

It uses Infrastructure as Code (usually Bicep or Terraform) to deploy the resources

## 3.4. Deploy an Application (azd deploy)

```
azd deploy
```

Once the resources are created, this command deploys your application to Azure

It takes care of both application code and configuration, ensuring everything is deployed to the right services

## 3.5. (OPTINAL) we run azd up"



## 4. We verify the deployment in Azure Portal



## 5. (OPTIONAL) We can create 


