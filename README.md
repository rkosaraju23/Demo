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