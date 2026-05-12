# Learning Terraform

Terraform is a DevOps tool for declarative infrastructure—infrastructure as code. It simplifies and accelerates the configuration of cloud-based environments. In this we will see how to use Terraform to configure infrastructure and manage resources with Amazon Web Services (AWS). After that we will see how Terraform manages your infrastructure, as well as how to use core Terraform commands. We will also delve into more advanced topics, including how to leverage code modules from the Terraform registry and how to create your own modules. 

# Resource Graph

It is used by terraform (directed acyclic graph)

# Terraform state

- keep the track of our infra state using state file (json formatted text file)

# Modules

- Bundle together a subset of code
- pass in arguments
- Work like custom resources
- All terraform code actually has at least one module (default module knonw as root)

## Module requirements

- main.tf file - contains the main code of module, a complex module might call out to other nested modules.
- variable.tf file - with input variables
- output.tf file - with output values like public dns.
- we can use remote sources like S3 bucket to use modules
- a module can have provider file.
- registry.terraform.io pre-made modules