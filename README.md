# ua-testrail

Please refer to the [ConnectALL Tech Docs](https://techdocs.broadcom.com/us/en/ca-enterprise-software/valueops/connectall/3-6/adapters/universal-adapter.html) for more information.

# Setup

## Supported Entities

This Universal Adapter currently supports the following entities:
* Suites, Sections, Test Cases, Test Plans, Runs, Tests 

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

Flow artifact type from a project in TestRail into another application (like ALM), and then update any changes (except can NOT create Tests within TestRail from another application).

# Known Limitations
keep Modified Date Field as updated_on
keep Date Time Format as yyyy-MM-dd'T'HH:mm:ss.SSS
keep Query Date Format as SECS_SINCE_UNIX_EPOCH
keep Issue Types
keep Fields with updated_on as Datetime DATATYPE
Query Modified Records: index.php?/api/v2/get_cases/${project_id}&updated_after=${last-modified-time}&limit=10&offset=0  has limit hardcoded as 10, and offset hardcoded as 0, modifiy accordingly if necessary.

# Supporting Documentation

Third Party API Documentation: https://support.testrail.com/hc/en-us/sections/7077185274644-API-reference
