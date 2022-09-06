# Random terraform configurations 🛠

This repository contains random terraform configuration files. Below is a detailed description of each file.

## Prerequisite

<a href="https://www.docker.com/" title="docker"><img src="https://github.com/get-icon/geticon/raw/master/icons/docker-icon.svg" alt="docker" width="30px" height="30px"></a>
<a href="https://www.terraform.io/" title="terraform"><img src="https://raw.githubusercontent.com/kreuzwerker/terraform-provider-docker/master/assets/terraform-logo.png" alt="docker" width="30px" height="30px"></a>

## File(s) 

- [Terraform file to provision NGINX server container with terraform.](https://github.com/kevinseq1/terraform-configurations/blob/main/tf-docker/main.tf)

## Usage
_Each directory in this repo consists of a different terraform configuration file. Once in the directory run the following commands.
- To initialize the directory
    ```
    terraform init
    ```
- To apply the configurations in the `.tf` file
    ```
    terraform apply
    ```
- To remove all the configurations applied from the `.tf` file.
    ```
    terraform destroy
    ```
