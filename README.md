# terraform_route53

Terraform module to create Route53 zones

## Variables

``` terraform
# name: the name of the route 53 zone
variable "example_org" { default = "example.org" }
```

## Terraform example

``` terraform
######################
# Route 53 variables
######################
variable "example_org" { default = "example.org" }

######################
# Route 53 zones
######################
module "example_org_route53" {
  source   = "git::https://github.com/virsas/terraform_route53.git?ref=v1.0.0"
  name     = var.example_org
}
```
