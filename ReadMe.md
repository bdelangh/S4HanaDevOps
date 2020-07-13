# Create a HANA DB via Azure DevOps & Terraform

## Prerequisite
* The terraform Extension for Azure DevOps needs to be installed.

## Setup
The following Azure Objects are created during deployment
- Resource Group : bdlSingleHANADevOp
- Network : 10.98.0.0/21
- SAP SID : HV1
- The deployment uses a Service Principal for this task. Currently the service principal bdl_terraform is used.
- [SPScripts](SPScripts) contains scripts to see the necessary environment variable for Terraform and Ansible when executing manual testing.
- Check Python version related to ansible : `ansible --version`
- Azure_rm.py needs execution rights: `chmod +x *.py`

## Further Information
* Tutorial on Azure DevOps and Terraform see [Automating infrastructure deployments in the Cloud with Terraform and Azure Pipelines](https://www.azuredevopslabs.com/labs/vstsextend/terraform/)
* Azure & Ansible Dynamic Inventory : [Configure dynamic inventories of your Azure resources using Ansible](https://docs.microsoft.com/en-us/azure/developer/ansible/dynamic-inventory-configure)

