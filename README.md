---
page_type: sample
languages:
- java
products:
- azure
description: "Azure Compute sample for assigning service identity to virtual machine scale set using newly created service principal."
urlFragment: compute-java-manage-scale-set-user-assigned-msi-from-service-principal
---

# Manage Scale Set User Assigned MSI From Service Principal (Java)


Azure Compute sample for assigning service identity to virtual machine scale set using newly created service principal.
  
- Create a VM scale-set
- Create a managed service identity #1 and create a service principal. Configure the service principal to have 2 permissions, to update the scale set and assign the managed service identity #1 to the scale set
- Create a managed service identity #2
- Login using created service principle and verify it can assign/remove identity #1, but not #2
 

## Running this sample

To run this sample:

Set the environment variable `AZURE_AUTH_LOCATION` with the full path for an auth file. See [how to create an auth file](https://github.com/Azure/azure-libraries-for-java/blob/master/AUTH.md).

```bash
git clone https://github.com/Azure-Samples/compute-java-manage-scale-set-user-assigned-msi-from-service-principal.git
cd compute-java-manage-scale-set-user-assigned-msi-from-service-principal
mvn clean compile exec:java
```

## More information

[http://azure.com/java](http://azure.com/java)

If you don't have a Microsoft Azure subscription you can get a FREE trial account [here](http://go.microsoft.com/fwlink/?LinkId=330212).

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
