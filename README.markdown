# Microsoft.AspNetCore.Authentication.OpenIdConnect and Microsoft.Identity.Web for authentication via Azure AD Project

This project uses Microsoft Identity Web, OpenID Connect, and Azure AD to authenticate users who can then access a web application.

## Azure AD

This project requires the settings of a provisioned Azure AD tenant. Configure the TenantId based on the supported account types of the registered Azure AD application.

## How to Use

Restore any necessary NuGet packages before building or deploying. Ensure that the settings in the appsettings.json are changed to point to match the settings of a provisioned Azure AD tenant. 

Build and run to start the MVC application on the default binding of https://localhost:44321

## Supported TenantId Settings

__Accounts in this organizational directory only__, replace this value with the directory (tenant) ID (a GUID) or the tenant name (for example, contoso.onmicrosoft.com)

__Accounts in any organizational directory__, replace this value with organizations

__All Microsoft account users__, leave this value as common


## Known Issues

In some cases the secured cookie used to persist authentication might need to be manually deleted before debugging the web project.

## Copyright and Ownership

All terms used are copyright to their original authors.

