In this project ,i will create two distinct, parallel environments against the same Terraform code using the terraform workspace command. i will also use the terraform state command to see what resources are being tracked in the state files of the different workspaces.

1 - Clone Terraform Code and Switch to the Proper Directory

2 - Create a New Workspace

3 - Deploy Infrastructure in the Test Workspace and Confirm Deployment via the AWS Management Console

4 - Deploy Infrastructure in the Default Workspace and Confirm Deployment via AWS Management Console

5 - Destroy Resources in the Workspaces and Delete the Test Workspace


#This folder is for the Terraform Workspace code.

# The main.tf file contains provider and EC2 VM resources
# and uses ${terraform.workspace} variable and logic to decide what 
# region to deploy in

#The network.tf file spins up the network resources required by
#the EC2 VM and uses ${terraform.workspace} variable to set their Names/IDs.


