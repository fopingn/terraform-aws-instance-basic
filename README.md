# AWS EC2 Instance Terraform light module

Terraform module which creates EC2 instance(s) on AWS.
## Usage

```hcl
module "ec2_sample" {
  source                 = "./instance"
  ami                    = "ami-00068cd7555f543d5"
  instance_type          = "t2.micro"
  monitoring             = true
  }
```
