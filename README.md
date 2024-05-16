terraform {
    required_providers {
        azurerm = {
            source = "Hashicorp\azurerm"
            version = " v 2.2.2"
        }
    }
}
provider "azurerm" {
    features {}
}

resource "azurerm_resource_group" "example" {
    name = "azure_rm"
    location = "east-us"
}

resource "azure_virtual_network" "example" {
    name = "azurerm_vnet"
    location = azurerm_resource_group_exampe.location
    resource_group = azurerm_resource_group_example.name
}
resource "azurerm_subnet" "example" {
   name = "azurerm_subnet"
   location = east-us

}
  
