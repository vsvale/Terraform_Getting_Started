# [Terraform_Getting_Started](https://app.pluralsight.com/library/courses/terraform-getting-started-2021)

Terraform is an amazing tool for automating infrastructure in the public and private cloud. This course will teach you the fundamentals of Terraform to deploy infrastructure in a consistent, repeatable manner across multiple services.

## Author

[Ned Bellavance](https://app.pluralsight.com/profile/author/edward-bellavance)

## Learning Platform

[Pluralsight](https://www.pluralsight.com/)

## Description
Systems Administrators and DevOps Engineers have always been charged to do more with less. Defining infrastructure in code and automating its deployment helps improve operational efficiency and lower administrative overhead. In this course, Terraform - Getting Started, you'll learn foundational knowledge of HashiCorp's Terraform software, a tool for infrastructure automation. First, you'll discover how to create and update a basic configuration. Next, you'll explore how to add variables, resources, and providers to expand your deployment. Finally, you'll learn how to leverage abstraction and improve code reuse with functions, state files, and modules. When you're finished with this course, you'll have the skills and knowledge of Terraform needed to write, plan, and create automated infrastructure deployments.

## Notes

### IaC
- Provisioning infrastructure through software to achieve consistent and predictable deployments
- Defined in code: json, yaml
- stored in source control: git
- Declarative
- Idempotent and consistent: if there is no change code and apply it again to the same enviroment, nothing will change
- push-type to the enviroment

#### Benefits of IaC
- Automated deployment
- Repeatable process
- Consistent environments
- Reusable components
- Documented architecture

## Terraform
- Infrastructure automation tool
- Open-source and vendor agnostic
- Declarative syntax
- HashiCorp configuration Language or JSON
- push-type to the enviroment

### Components
- Executable
- Configuration files
- Provider plugins
- State data: current information in target enviroment

### Block Syntax
```
block_type "label" "name_label"{
    key = "value"
    nested_block {
        key = "value"
    }
}
```

### Execise Files
https://github.com/ned1313/Getting-Started-Terraform

### Install

- `wget -O- https://apt.releases.hashicorp.com/gpg | gpg --dearmor | sudo tee /usr/share/keyrings/hashicorp-archive-keyring.gpg`
- `echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list`
- `sudo apt update && sudo apt install terraform`
- `terraform version`

### Labs
Follow commands to create a develop enviroment in AWS to Globalmantics