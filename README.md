# Random terraform configurations 🛠

This repository contains random terraform configuration files. Below is a detailed description of each file.

## Prerequisite

<a href="https://www.docker.com/" title="docker"><img src="https://github.com/get-icon/geticon/raw/master/icons/docker-icon.svg" alt="docker" width="30px" height="30px"></a>
<a href="https://www.terraform.io/" title="terraform"><img src="https://raw.githubusercontent.com/kreuzwerker/terraform-provider-docker/master/assets/terraform-logo.png" alt="terraform" width="30px" height="30px"></a>
<a href="https://www.aws.com/" title="aws"><img src="https://a0.awsstatic.com/main/images/logos/aws_smile-header-desktop-en-white_59x35@2x.png" alt="aws" height="25px"></a>

## File(s) 

- [Terraform file to provision NGINX server container with terraform.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-docker/main.tf)
- [Terraform file to provision an EC2 instance in a given region and subnet in AWS.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/main.tf)
- [Terraform file to provision two SNS topics in two different regions using terraform providers.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/main2.tf)
- [Terraform file to provision an EC2 instance and install a webserver on it using provisioners.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/main3.tf)\
 \* Additional configurations can be found in [state3.tf](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/state3.tf) file.

## Usage
- _Each directory in this repo consists of a different terraform configuration files in sub directories. (When running the following commands make sure only one `main.tf` is present in the directory and rename any `.tf` file to `main.tf` while using that configuration file)_

- Enable verbose output logging for Terraform commands using:
    ```
    export TF_LOG=TRACE
    ```

- To initialize the directory:
    ```
    terraform init
    ```
- To validate the code to look for any errors in syntax, parameters, or attributes within Terraform resources that may prevent it from deploying correctly:
    ```
    terraform validate
    ```
- To view what the configuration in the `.tf` file will create:
    ```
    terraform plan
    ```
- To apply the configurations in the `.tf` file:
    ```
    terraform apply --auto-approve
    ```
- To remove all the configurations applied from the `.tf` file:
    ```
    terraform destroy --auto-approve
    ```
