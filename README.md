# Terraspace Azure Windows Virtual Machine Example

This project shows how to create an [Azure Windows Virtual Machine](https://www.terraform.io/docs/providers/azurerm/r/windows_virtual_machine.html) with [Terraspace](https://terraspace.cloud/).

## Setup

    git clone https://github.com/boltops-tools/terraspace-azurerm-windows-vm
    cd terraspace-azurerm-windows-vm
    bundle

## Deploy

Make sure the `ARM_CLIENT_ID` and `ARM_CLIENT_SECRET` env variables are set:

Terraspace Docs: [Configure Azure](https://terraspace.cloud/docs/learn/azure/configure/)

You also want to set your region.

    az configure --defaults location=eastus

Then to deploy:

    terraspace up windows-vm

A Virtual Machine named `windows-vm` is created. Note, there is a 15-character limit on Windows Machine names.

## About

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

[Terraspace](https://terraspace.cloud/) and this project was built by [BoltOps](https://www.boltops.com). We also offer:

* [Paid Consulting Services](https://www.boltops.com/consulting)
* [BoltOps Pro: Infrastructure Code as a Service](https://www.boltops.com/pro)
