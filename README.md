# tfmod_route53

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
module "virsas_com_route53" {
  source   = "github.com/virsas/tfmod_route53"
  name     = var.example_org
}
```
