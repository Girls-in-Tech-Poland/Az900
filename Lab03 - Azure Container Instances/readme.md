# Lab03 - Azure Container Instances

This lab aims to provide a hands-on experience in deploying a container instance using the [Azure Container Instances](https://azure.microsoft.com/en-us/services/container-instances/) (ACI)

## Deployment methods

### Azure Portal (Manual)

> This method aims to deploy an ACI instance using the Azure Portal

- Azure Portal
    - Sign in to the portal using the provided credentials
- Resource Group
    - Create a dedicated resource group to host your azure container instance
- Create the Azure Container Instance
    ![create-resource](./img/01-create-resource.png)
    - Select `Create a resource`
    - Search the Marketplace for `Container Instances`
    ![create](./img/02-create.png)
    - Click `Create`
- Configure ACI Basics
    ![configure-aci-basics](./img/03-configure-aci-basics.png)
    - `Resource group`: Ensure the recently created resource group is selected
    - `Container name`: provide a name for the container
    - `Region`: pick a region
    - `Image type`: ensure `Public` is set
    - `Image name`: set to `mcr.microsoft.com/azuredocs/aci-helloworld:latest`
    > If you have **docker** installed, you can test if the image is available with `docker pull mcr.microsoft.com/azuredocs/aci-helloworld:latest`
    - `OS type`: ensure `Linux` is selected
    - `Size`: use the default value
    - Click `Next: Networking`