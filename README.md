# Azure Infrastructure Deployment with Terraform

This Terraform configuration defines the infrastructure components required for a basic setup on Microsoft Azure. The setup includes a virtual network, public IPs, subnets, network interfaces, network security groups, Linux virtual machines, and an application gateway.

## Prerequisites

Before running this Terraform script, ensure that you have:

1. **Terraform Installed:** If not, download and install Terraform from [Terraform Downloads](https://www.terraform.io/downloads.html).

2. **Azure Subscription:** You need an active Azure subscription.

3. **Azure CLI or Azure PowerShell:** You should have the Azure CLI or Azure PowerShell installed on your machine and authenticated with your Azure subscription.

## How to Use

1. Clone this repository:

   ```bash
   git clone <repository-url>
2. Change into the project directory:
   ```bash
   cd <project-directory>
3. Initialize Terraform:
   ```bash
   terraform init
4. Review the terraform plan:
   ```bash
   terraform plan
5. Apply the Terraform plan to create Azure resources:
   ```bash
   terraform apply
## Configuration Customization
This Terraform script uses variables for configuration. You can customize the configuration by updating the variables.tf file or by providing values through a separate .tfvars file.
### Example .tfvars File
resource_group_name = "myResourceGroup"
vnet_name           = "myVNet"
### Example Usage
terraform apply -var-file=myconfig.tfvars

## Cleanup
If you want to destroy the resources created by Terraform and clean up the Azure environment:

   ```bash
   terraform destroy


