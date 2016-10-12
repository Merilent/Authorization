# Authorization #

Authorization framework provides the flexibility to authorize user/group. It generates tokens for the authenticated users and adds application roles assigned to the user into the database. Using this we can display user-specific UI, provide access control over the application, etc.

### This project consists of: ###

  * **Merilent.Authorization** : Authorization framework library.
  * **AuthorizationApp**       : Utility app for the admin to check the Roles assigned to a user to access application.
  * **AuthorizationDB**        : Database project having tables and views consisting of Roles accessible to a user/group.
  * **Sample Application**     : Sample application using Authorization framework.


## Getting started ##
### Import Database ###
 
Import database project and create a database on your Database Server to configure the user Roles.

**Note**: Create all the objects that are available in the project database on your Server Database too.

## Pre-Requisites ##

While ADFS service provides Single Sign - On (SSO) experience, below are a few points we need to consider in order to make the experience seamless.

#### Common pre-requisites ####

* Any of the current Web browsers with JScript enabled can work as an ADFS client.
* Cookies must be enabled, or at least trusted, for the federation servers and Web applications that are being accessed. It’s by using Cookies that we prevent repeated logons to a service, within the same session. Cookies can also prevent repeated home realm discovery prompts with that are more claim providers on the STS. 
* The authentication cookie is signed but not encrypted, which is one reason why use of TLS/SSL is mandatory in ADFS i.e. SSL Certificate is required (compulsory https).

#### Server Requirement ####

The following technologies are required:

* Windows Server for ADFS Installation.
* SQL Server for ADFS configuration table.
* AD for attribute storage.

#### Browser Requirement ####

When AD FS authentication is performed via a browser or browser control, your browser must comply to the following requirements:

* JScript must be enabled.
* Cookies must be turned on.
* For user certificate & device certificate authentication (Workplace Join functionality), the browser must support SSL client    certificate authentication.


For more information please refer to the detailed [documentation](https://github.com/Merilent/Authorization/wiki)



