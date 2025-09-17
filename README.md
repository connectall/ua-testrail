# ua-testrail

Please refer to the [ConnectALL Tech Docs](https://techdocs.broadcom.com/us/en/ca-enterprise-software/valueops/connectall/3-6/adapters/universal-adapter.html) for more information.

# Setup

## Supported Entities

This Universal Adapter currently supports the following entities:
* Test Cases

*Note: This Universal Adapter is provided as-is. It is tested and validated using the entities and configurations as defined. Any additional customizations are not supported and should be made at your own discretion.*

## Connection Details

* **Connection Name:** *Name of Application*
* **Application Type:** TestRail
* **URL:** https://xxx.testrail.io (replace xxx with your specific)
* **User Name:** User Name
* **Password:** User's password
* **Application Category:** *Pick from dropdown list*
* **Time Zone:** UTC
* **Select Group:** *Set if neccessary*
* **Auth Option:** Header
* **Authentication Type:** Basic
* **API Key:** Leave Blank
* **API Value:** Leave Blank

## Flow Filters

## Example Automation

Flow Test Case from a project in TestRail into another application (like Rally), and then update any changes (uni or bidirectional).

# Known Limitations
keep Modified Date Field as updated_on
keep Date Time Format as yyyy-MM-dd'T'HH:mm:ss.SSS
keep Query Date Format as SECS_SINCE_UNIX_EPOCH
set MetaData project_id value
keep Issue Type as TestCase
keep Fields with updated_on as Datetime DATATYPE

# Supporting Documentation

Third Party API Documentation: [Link to API Documentation]([https://learn.microsoft.com/en-us/rest/api/azure/devops/processes/lists/list?view=azure-devops-rest-7.1](https://support.testrail.com/hc/en-us/articles/15762591438996-Exporting-test-cases#getting-test-cases-0-0))
