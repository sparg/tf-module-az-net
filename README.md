## Module networking

### Structure
- **main.tf**
- **variables.tf**
- **outputs.tf**

### Usage module

Networking
```hcl
module "network" {
  source = "git@github.com:Sparg/tf-module-az-net.git?ref=v1.0.0"

  address_space         = var.address_space
  subnet_address_prefix = var.subnet_address_prefix
  location              = var.location
  resource_group_name   = var.resource_group
  instance              = var.instance
  environment           = var.environment
}
```

### Outputs module

Networking
- `subnet_id`
