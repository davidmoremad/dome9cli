# Dome9 CLI

[![Test](https://github.com/davidmoremad/dome9cli/actions/workflows/test.yaml/badge.svg)](https://github.com/davidmoremad/dome9cli/actions/workflows/test.yaml)

This Command Line Interface (CLI) is a set of commands used to create and manage Dome9 resources.
Developed to facilitate the daily use and help to work in agile methodologies (continuous-integration)
This package consumes calls through the Dome9 Python SDK so it contains the same methods.

This CLI helps to work on Dome9 from our different agile services like Jenkins, Github or Travis, creating new rulesets, running
assessments or listing our protected assets.

To install:
```
pip install --user dome9cli
dome9cli --help
```

## Commands

```
Usage: dome9cli <command> <arguments>

```

#### create_ruleset  
Description: Create a compliance ruleset  
Command: `.\dome9cli.py create_ruleset jsonFile`  


#### delete_exclusion  
Description: Delete a specific exclusion  
Command: `.\dome9cli.py delete_exclusion id=0`  


#### delete_remediation  
Description: Delete a specific remediation  
Command: `.\dome9cli.py delete_remediation id=0`  


#### delete_ruleset  
Description: Delete a specific ruleset  
Command: `.\dome9cli.py delete_ruleset id=0`  


#### generate_ruleset  
Description: Generate a ruleset template  
Command: `.\dome9cli.py generate_ruleset name=minimum, cloud=aws, rulesFile='./rules.json', desc='My description'`  


#### get_cloud_account  
Description: Get a specific cloud account  
Command: `.\dome9cli.py get_cloud_account id=0`  


#### get_ruleset  
Description: Get a specific compliance ruleset  
Command: `.\dome9cli.py get_ruleset id=0`  


#### list_aws_accounts  
Description: List AWS Cloud accounts  
Command: `.\dome9cli.py list_aws_accounts`  


#### list_azure_accounts  
Description: List Azure Cloud accounts  
Command: `.\dome9cli.py list_azure_accounts`  


#### list_cloud_accounts  
Description: List all cloud accounts (AWS, Azure, GCP and Kubernetes)  
Command: `.\dome9cli.py list_cloud_accounts`  


#### list_exclusions  
Description: List all exclusions  
Command: `.\dome9cli.py list_exclusions`  


#### list_google_accounts  
Description: List Google Cloud accounts  
Command: `.\dome9cli.py list_google_accounts`  


#### list_kubernetes_accounts  
Description: List Kubernetes accounts  
Command: `.\dome9cli.py list_kubernetes_accounts`  


#### list_remediations  
Description: List all remediations  
Command: `.\dome9cli.py list_remediations`  


#### list_rulesets  
Description: List compliance rulesets  
Command: `.\dome9cli.py list_rulesets`  


####  run_assessment  
Description: Run assessment and get report URL  
Command: `.\dome9cli.py run_assessment rulesetId=0, cloudAccountId=0000-0000-0000-0000`  
