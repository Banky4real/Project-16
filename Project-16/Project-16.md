## **Documentation for Project 16**

### Automate Infrastructure With IAC using Terraform Part 1

### Creating an IAM User with Programatic access

![IAM-User-created-with-programatic-access](./Images/IAM-User-created-with-programatic-access.png)

### Boto3 Installation

![Installing-Boto3](./Images/boto3-installation.png)

### Installing AWS CLI

![installing-aws-cli](./Images/installing-aws-cli.png)

### Configuring my credentials for CLI to authenticate with AWS and also for terraform to Authenticate with AWS

![configuring-CLI-and-terraform-to-Authenticate-with-AWS](./Images/configuring-CLI-and-terraform-to-Authenticate-with-AWS.png)

### Creating S3 Bucket

![creating-S3-Bucket](./Images/creating-S3-Bucket.png)

### Ran AWS s3 LS on CLI to List the bucket i've just created

`aws s3 ls`
![creating-S3-Bucket](./Images/Aws-s3-bucket-List-CLI.png)

### Initializing Terraform in our working Directory

![terraform-initialized-in-our-working-directory](./Images/terraform-initialized-in-our-working-directory.png)

### Specifying our Provider and Creating a VPC

![creating-a-vpc-and-specifying-our-provider](./Images/creating-a-vpc-and-specifying-our-provider.png)

### Running Terraform Plan to show the resource that is about to be Created

![terraform-plan-to-show-VPC-resource-that-is-about-to-be-created](./Images/terraform-plan-to-show-VPC-resource-that-is-about-to-be-created.png)

### Creating our Subnets resource
`terraform plan`

![terraform-plan-to-create-subnets](./Images/terraform-plan-to-create-subnets.png)

`terraform apply`

![terraform-apply-to-create-subnets](./Images/terraform-apply-to-create-subnets.png)

### VPC Created
![vpc-created-after-apply](./Images/vpc-created-after-apply.png)

### 2 Public Subnets Created after apply
![two-public-subnets-created-after-terraform-apply](./Images/two-public-subnets-created-after-terraform-apply.png)

### Destroying the resources created
`terraform destroy`
![terraform-destroy-to-delete-the-resources-created](./Images/terraform-destroy-to-delete-the-resources-created.png)

### Refactoring pur Code by Fixing Hard Coded Values

### Creating a Variables.tf file to keep variables for our Hardcoded Values
![Variables-to-fix-our-hard-coded-values](./Images/Variables-to-fix-our-hard-coded-values.png)

### Fixing multiple resource blocks

### Creating a Datasource.tf file to keep our datasource variables which will fetch data from AWS for available resources

![datasource-variable-to-get-list-of-available-resources](./Images/datasource-variable-to-get-list-of-available-resources.png)

### Refferencing our Variables in Main.tf file

![variables-refferenced-in-main-tf-file](./Images/variables-refferenced-in-main-tf-file.png)

### Removing hardcoded count value for our multiple subnet creation using length() function

![fixing-hardcoded-count-value](./Images/fixing-hardcoded-count-value.png)

### Declaring a variable to store the desired number of public subnets we need and setting the default value.

![variable-to-declare-the-desired-number-of-public-subnet-we-want](./Images/variable-to-declare-the-desired-number-of-public-subnet-we-want.png)

### Refferencing the variable for our preffered number of public subnet in our Main.tf file

![refferencing-the-variable-in-our-main-tf-file](./Images/refferencing-the-variable-in-our-main-tf-file.png)

### Terraform format to arrange our code
`terraform fmt`

![refferencing-the-variable-in-our-main-tf-file](./Images/terraform-fmt-to-arrange-our-code-for-us.png)

### Terraform apply with --auto-approve to create our resources

![terraform-apply-with-auto-approve-to-create-our-resources](./Images/terraform-apply-with-auto-approve-to-create-our-resources.png)

### Resources Created

![vpc-created](./Images/vpc-created.png)

![subnets-created](./Images/subnets-created.png)