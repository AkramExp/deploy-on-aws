# Deploy on AWS




## Description
In this DevOps project I used **Terraform**, **Ansible** and **Docker Compose** tools.

- Provisioned **AWS Cloud vpcs, subnets, gateways, routing tables, security group and EC2** instance with the help of terraform files.

- Made 2 terraform modules as subnet to provision subnet resources and webserver to provision servers so the code shud be resusable without writing repetative stuff and imported those modules into main.tf file.

- With Ansible I first installed python3, docker and docker compose on AWS EC2 instance then copied the neccessary files to the server to run the application.

- Application run with docker compose configured in ansible playbook.


## Installation

Provision EC2 instance with terraform

```bash
    cd terraform
    terraform init
    terraform apply --auto-approve
```
Run ansible playbook
```bash
    cd ansible
    ansible-playbook deploy-docker.yaml
```

    
