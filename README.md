# Created a dev environment with on-demand deployment to Azure with Terraform
![azure-tf](https://github.com/d-hearn/terraform-azure-tutorial/assets/141779135/fbb484e8-a5b1-4b59-b3fe-ce5f5f288450)

In order to learn the basics and get a better understanding of how to use Terraform, I created a simple configuration consisting of:
- Resource group
- VNet and Subnet
- Public IP
- Virtual Machine

3 files were created to complete the config keeping orginization and ease of management in mind.
  - `main.tf` - This is where the resources are defined using the `azurerm` provider to deploy to Azure
  - `customdata.tpl` - Adding a bash script to this file, Docker will be installed on the VM at the time of deployment.
  - `windows-ssh-script.tpl` - I used Remote-SSH in VS Code in order to log in and use the VM through VS Code. This is where I stored the script required to do so.

