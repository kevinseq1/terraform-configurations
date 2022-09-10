# Random terraform configurations 🛠

This repository contains random terraform configuration files. Below is a detailed description of each file.

## Prerequisite

<a href="https://www.docker.com/" title="docker"><img src="https://github.com/get-icon/geticon/raw/master/icons/docker-icon.svg" alt="docker" width="30px" height="30px"></a>
<a href="https://www.terraform.io/" title="terraform"><img src="https://raw.githubusercontent.com/kreuzwerker/terraform-provider-docker/master/assets/terraform-logo.png" alt="docker" width="30px" height="30px"></a>

## File(s) 

- [Terraform file to provision NGINX server container with terraform.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-docker/main.tf)
- [Terraform file to provision an EC2 instance in a given region and subnet in AWS.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/main.tf)
- [Terraform file to provision two SNS topics in two different regions using terraform providers.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-aws/main2.tf)

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
