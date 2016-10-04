# Authorization #

Authorization framework provides the flexibility to authorize user/groups. It generates token for authenticated user and adds application roles assign to user in databases. Using this we can also display user specific UI, include access control on Application, etc.

### This project have ###

  * **Merilent.Authorization** : It is a Authorization framework library.
  * **AuthorizationApp**       : It is a utility app for admin to check user having which roles to access applicaition.
  * **AuthorizationDB**        : It is a Database project having tables and view for Roles access to user or group.
  * **Sample Application**     : It has sample applicaiton using Auhtorization framework.


## Getting started ##
### Import Database ###
 
Import databse project and create database to configure user Roles on your Databse Server.

**Note**: Create all object availbale in database project on your Databse Server.

## Pre-Requisites ##

While ADFS service provides Single Sign On (SSO) experience, below are a few points we need to be aware of to make the experience       seamless.

#### Common pre-requisites ####

* Although any current Web browser with JScript enabled can work as an ADFS client.
* Cookies must be enabled, or at least trusted, for the federation servers and Web applications that are being accessed. It’s using  Cookies that we prevent repeated logons to a service, within the same session. Cookies can also prevent repeated home realm discovery prompts with that are more claim providers on the STS.
* The authentication cookie is signed but not encrypted, which is one reason why use of TLS/SSL is mandatory in ADFS i.e. SSL Certificate is required (compulsory https).

#### Server Requirement ####

The following technologies are required.

* Windows Server for ADFS Installation and SQL Server for ADFS configuration table.
* AD for attribute store.

#### Browser Requirement ####

When AD FS authentication is performed via a browser or browser control, your browser must comply to the following requirements:

* JavaScript must be enabled
* Cookies must be turned on
* For user certificate & device certificate authentication (workplace join functionality), the browser must support SSL client    certificate authentication


For more information please refer [documentation](https://github.com/Merilent/Authorization/wiki)



