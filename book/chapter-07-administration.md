# General Bots Administration

## Commands

General Bot can be controlled by the same chat window people talk to, so
here is a list of admin commands related to deploying .gb* files.

| Command         | Description                                                                                                     |
|-----------------|-----------------------------------------------------------------------------------------------------------------|
| deployPackage   | Deploy a KB package. Usage **deployPackage** [package-name]. Then, you need to run rebuildIndex.                |
| undeployPackage | Undeploy a KB. Usage **undeployPackage** [package-name].                                                        |
| redeployPackage | Undeploy and then deploys the KB. Usage **redeployPackage** [package-name]. Then, you need to run rebuildIndex. |
| setupSecurity   | Setup connection to user directories.                                                                           |

Discontinued commands:

| Command      | Description                                                                               | Reason                         |
|--------------|-------------------------------------------------------------------------------------------|--------------------------------|
| rebuildIndex | Rebuild Azure Search indexes, must be run after **deployPackage** or **redeployPackage**. | Now it is called automatically |

## Enviroment Variables Reference

| Name                   | Sample Value                                     | Description |
|------------------------|--------------------------------------------------|-------------|
| ADDITIONAL_DEPLOY_PATH | D:\data\gbai                                     | Deploy folder to look for packages. 
| ADMIN_PASS             | E732+!#xJ3a_*!                                   | Administration password for the conversational interface.
| CLOUD_SUBSCRIPTIONID   | 622e5037-f7f1-49f6-a9c4-28babbb0fs               | Cloud subscription ID used to deploy new bots.
| CLOUD_LOCATION         | westus                                           | Cloud location used to deploy new bots.
| CLOUD_GROUP            | newassistant                                     | Cloud group used to deploy new bots.
| CLOUD_USERNAME         | someone@domain                                   | Cloud username used to deploy new bots.
| CLOUD_PASSWORD         | x@8k*p!93aZ0_*!                                  | Cloud password used to deploy new bots.
| MARKETPLACE_ID         | 9c90ff1c3-101b-4f0d-85cd-4bada2226fe3            | Martplace identifier associated to the boot bot.
| MARKETPLACE_SECRET     | nzrNUUG6214%raqzYWQ8(+%                          | Martplace password associated to the boot bot.
| NLP_AUTHORING_KEY      | 0aa343b06d044b66a2159abf080ff1c3                 | The key from NLP service allowing creating of bot NLP libraries.
| STORAGE_DIALECT        | mssql                                            | The bot database dialect configuration value. Can be MSSQL or SQLITE.
| STORAGE_SERVER         | newassistant-storage-server.database.windows.net | The bot database server name configuration value.
| STORAGE_NAME           | newassistant-storage                             | The bot database database name configuration value.
| STORAGE_USERNAME       | sahaaksfqiehke                                   | The bot database security username configuration value.
| STORAGE_PASSWORD       | 8adk9dio378!P                                    | The bot database security password configuration value.
| STORAGE_SYNC           | true                                             | If the bot server should sync database before running.

## How to

### Move to production (Azure)

* Update bot endpoint;

## Bot Analytics

## Cloud Internals


