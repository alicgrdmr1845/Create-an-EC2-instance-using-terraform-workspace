## This project is about creating EC2 instances for test and development workspaces
-Variable file created for each environment
-Local command used for simple tagging 
-Tag command used for tagging EC2 instance for each environment.
-Don t forget to fill the necessary security credentials in the provider section. It s deleted from my code block because of security issues. 

![Alt text](C/terraform/terraform-workspaces/worksapces.png "created instances")

#Bash commands 
-terraform workspace new dev (for creating dev environment)
-terraform workspace list (listing workspaces)
-terraform workspace show (shows which workspace you are in)
-terraform workspace select (helps you to move between environment workspaces you have)
-terrafom init 
-terraform plan -var-file ="dev.tfvars"
-terraform apply -var-file ="dev.tfvars"
-terraform destroy (you must be in the workspace that you want to delete, because workspaces stay in isolatedform each other)
