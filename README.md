# terraform-azure-public-ip

Terraform module that manages an Azure Public IP Address.
It is based on the official [```azurerm_public_ip``` resource](https://www.terraform.io/docs/providers/azurerm/r/public_ip.html) from ```azurerm``` provider.

## Example usage

```hcl
inputs = {
    name = "custom-ip-address"
    resource_group_name = "myresourcegroup"
    allocation_method = "Dynamic"
    sku = "Basic"

    domain_name_label = "my-domain"

    tags = {
        "environment" = "dev"
        "client" = "scalair"
    }
}
```
