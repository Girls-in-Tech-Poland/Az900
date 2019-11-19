# Lab05 - Azure Blob Storage

![logo](./img/00-logo.svg)

This lab aims to provide a hands-on experience in deploying an Azure Storage Account containing a Container with BLobs

## About the exercise

The purpose of the exercise is to demonstrate the deployment of a storage account, creation of a container and upload of a file to the blob storage

## Deployment

### Azure Portal (Manual)

> This method aims to deploy an ACI instance using the Azure Portal

#### Azure Portal

- Sign in to the portal using the provided credentials.
#### Resource Group

- The resource group dedicated for this lab is: `AZ900_user[i]_LAB05_RG`

#### Create the Storage Account
![create-resource](./img/01-create-resource.png)
- Select `Create a resource`.
- Search the Marketplace for `Storage account`.
![create](./img/02-create.png)
- Click `Create`.

#### Configure Storage Account Basics
 
![configure-basics](./img/03-configure-basics.png)
- **Resource group**: Ensure the `AZ900_user[i]_LAB05_RG` resource group is selected.
- **Storage account name**: set to a unique value.
- **Location**: pick a region.
- **Performance**: set to `Standard`
- **Account kind**: ensure `StorageV2` is set.
- **Replication**: set to `Locally-redundant storage (LRS)`.
- **Access tier**: set to `Hot`
- Click `Review + create` and then `Create` after validation is successful.

#### The Storage Account deployment
![deployment](./img/04-deployment.png)
*Storage account deployment underway*

![deployment-completed](./img/05-deployment-completed.png)
*Storage account deployment completed*
- Wait for the resource deployment to complete successfully.
- Click `Go oto resource` when deployment is completed.

#### The Container Creation

![overview](./img/06-overview.png)
- Click on `Containers`

![add-container](./img/07-add-container.png)
- Click on `+ Container`

![configure-container](./img/08-configure-container.png)
- **Name**: set to `images`
- **Public access level**: set to `Container`
- Ignore the warning
- Click on `Ok`
- Wait for the container creation to complete
- Click on the newly created container

#### File upload to Blob
![upload](./img/09-upload.png)
- Click on `Upload`
- Right-hand side flyout-menu will appear

![upload-blob](./img/10-upload-blob.png)
- Click on the folder icon
- Select an image to upload
- Wait for `Upload` to become accessible
- Click on `Upload`
- Click on the newly uploaded file

![](./img/11-img-url.png)
- Click on the copy button to copy the img URL to clipboard
- Open a new tab in your browser
- Paste the image URL and press ENTER
- The image should be accessible from a public blob

## Clean up
Now simply delete resource LAB05 resource group.
