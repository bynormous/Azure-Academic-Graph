# Microsoft Academic Graph Guide #

The Microsoft Academic Graph (MAG) is a heterogeneous graph containing scientific publication records, citation relationships between those publications, as well as authors, institutions, journals, conferences, and fields of study. This graph is used to power experiences in Bing, Cortana, Word, and in Microsoft Academic. The graph is currently being updated on a weekly basis. 

## Table of content ##

1. Prerequisite
2. Get Microsoft Academic Graph on Azure storage
3. Sign up for MAG provisioning
4. Recommended analytics options

## Prerequisite

### Azure Subscription

Please create a new Azure subscription for the distribution previews. If your organization already using Azure, this could be a separate subscription under the same tenant id. If you start from scratch, for example “create Azure free account”, the subscription will be created under a new tenant id.

## Get Microsoft Academic Graph on Azure storage ##

### Create an Azure Storage Account ###

1. Azure Portal > Create a resource > Storage > Storage account

    ![Alt text](https://docs.microsoft.com/en-us/academic-services/graph/media/create-storage-account/select.png)


2.  Provide following values to create an Azure Storage account. Then click "Review + create" button.

    |Property  |Description  |
    |---------|---------|
    |**Subscription** | From the drop-down, select your Azure subscription. |
    |**Resource group** | Specify whether you want to create a new resource group or use an existing one. A resource group is a container that holds related resources for an Azure solution. For more information, see [Azure Resource Group overview](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-overview). |
    |**Storage account name** | Provide a name for your Databricks workspace, e.g. **magas<org_name>**. You don’t need to use your organization name after the "magas", however the account name must be unique among all Azure Storage Accounts. |
    |**Location**    | Select whatever location (region) that is most appropriate for your existing Azure resources |
    |**Performance** | Standard |
    |**Account kind**| StorageV2 (general purpose v2) |
    |**Replication** | LRS |
    |**Access tier** | Cool |

    ![Enter details for new storage account resource](https://docs.microsoft.com/en-us/academic-services/graph/media/create-storage-account/details.png "Enter details for new storage account resource")

3. Verify that the information you entered is correct and click the "create" button

    ![Submit new storage account resource for creation](https://docs.microsoft.com/en-us/academic-services/graph/media/create-storage-account/submit.png "Submit new storage account resource for creation")

### Note Azure storage account name and primary key

1. Once notified that the storage account has been created, click “go to resource”

    ![Navigate to the new storage account resource](https://docs.microsoft.com/en-us/academic-services/graph/media/create-storage-account/go-to-resource.png "Navigate to the new storage account resource")

2. Go to “access keys” and take note of the “storage account name” and the “primary key”

    ![Save new storage account resource name and access keys for later](https://docs.microsoft.com/en-us/academic-services/graph/media/create-storage-account/access-keys.png "Save new storage account resource name and access keys for later")

3. Make sure that you have these items of information:

   * The name of your Azure Storage (AS) account.

   * The access key of Azure Storage (AS) account.

## Sign up for MAG provisioning ##

To sign up for MAG on AS distribution preview, send the following information using your school or company email account to <a href="mailto:academicapi@microsoft.com?subject=Access request to Microsoft Academic Graph (MAG) on Azure Storage (AS) distribution preview">academicapi@microsoft.com</a> with the subject "Access request to Microsoft Academic Graph (MAG) on Azure Storage (AS) distribution preview":

- Are you affiliated with a company or university?
  - If company, please provide the company’s name, your department/group and your role
  - If university, please provide the university’s name, department, group/advisor, and your role (undergraduate student, grad student, professor, etc.)
- Brief description of the project you will be using MAG for
- Name of your Microsoft sales representative, if you have one
- Azure Storage (AS) account name
- Azure Storage (AS) account primary access key
- Which type of provisioning model you want:
  1. One-time provisioning of the most recent MAG release
  1. Automatic provisioning of each new MAG release (~every 1-2 weeks)

> **NOTE**
>
> MAG is currently in a free preview period, so there are no charges associated with the provisioning or use of the data/service itself. However Azure requires you to cover all costs associated with standard resource creation, usage, etc. For cost estimates associated with MAG please see the [Pricing](https://docs.microsoft.com/en-us/academic-services/graph/resources-pricing) page. <br/><br/>Most research institutions have an "Enterprise Account" with Microsoft including Azure subscription. The pricing for Enterprise Accounts differ from the individual account shown in Azure's price calculator. <br/><br/>If you have an Enterprise Account, please check with your individual institution's Information Technology/Computer Center resource on the process of setting up Azure to get MAG. You might need to obtain a "Master Agreement #" and involve MLSP (Microsoft Licensed Solution Provider) for help.
