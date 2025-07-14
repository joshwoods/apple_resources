

- App Store Connect API
-  UserRole 

Type

# UserRole

Strings that represent user roles and permissions in App Store Connect.

App Store Connect API 1.0+

``` source
string UserRole
```

## Possible Values 

`ADMIN`  

`FINANCE`  

`ACCOUNT_HOLDER`  

`SALES`  

`MARKETING`  

`APP_MANAGER`  

`DEVELOPER`  

`ACCESS_TO_REPORTS`  

`CUSTOMER_SUPPORT`  

`CREATE_APPS`  

`CLOUD_MANAGED_DEVELOPER_ID`  

`CLOUD_MANAGED_APP_DISTRIBUTION`  

`GENERATE_INDIVIDUAL_KEYS`  

## Mentioned in 

App Store Connect API 3.5 release notes

App Store Connect API 1.4 release notes

Creating auto-renewable subscription groups

Creating and configuring win-back offers

Managing in-app purchases

## Possible values

ACCESS_TO_REPORTS  
Permission to download reports associated with a role. The Access To Reports permission is an additional permission for users with the App Manager, Developer, Marketing, or Sales role. If you add this permission, the user has access to all of your apps.

ACCOUNT_HOLDER  
Role responsible for entering into legal agreements with Apple. The person who completes program enrollment has the Account Holder role in their Apple Developer account and their App Store Connect account.

ADMIN  
Role that serves as a secondary contact for teams and has many of the same responsibilities as the Account Holder role. Admins have access to all apps.

APP_MANAGER  
Role that manages all aspects of an app, such as pricing, App Store information, and app development and delivery.

CLOUD_MANAGED_APP_DISTRIBUTION  
Permission to submit requests for apps and software to be signed by a cloud- termmanaged Apple Distribution certificate. App Store Connect automatically creates a certificate if one doesn’t exist. The system grants this permission by default to Account Holder and Admin roles. Account Holder, Admin, and App Manager roles may grant access to this permission to other users with App Manager or Developer roles. This permission requires that the user has access to Certificates, Identifiers & Profiles.

CLOUD_MANAGED_DEVELOPER_ID  
Permission to submit requests for apps and software to be cloud signed by a cloud- termmanaged Developer ID certificate. App Store Connect automatically creates a certificate if one doesn’t exist. The system grants this permission by default to the Account Holder role. The Account Holder may grant access to this permission to users with the Admin role, who may grant it to other Admins. This permission requires that the user has access to Certificates, Identifiers & Profiles.

CREATE_APPS  
A permission that enables users with Developer or Marketing roles to create app records.

CUSTOMER_SUPPORT  
Role that analyzes and responds to customer reviews on the App Store. If a user has only the Customer Support role, they go straight to the Ratings and Reviews section when they click on an app in My Apps.

DEVELOPER  
Role that manages development and delivery of an app.

FINANCE  
Role that manages financial information, including reports and tax forms. A user that has this role can view all apps in Payments and Financial Reports, Sales and Trends, and App Analytics.

MARKETING  
Role that manages marketing materials and promotional artwork. If an app is in consideration to be featured on the App Store, Apple contacts the user with this role.

SALES  
Role that analyzes sales, downloads, and other analytics for the app.

GENERATE_INDIVIDUAL_KEYS  
Role that allows a user to generate an individual API key.

## Discussion

For more information about roles and permissions, see Program Roles.

## See Also

### Objects and Data Types

object User

The data structure that represents a Users resource.

object UserUpdateRequest

The request body you use to update a User.

object UserResponse

A response that contains a single Users resource.

object UsersResponse

A response that contains a list of Users resources.

object UserVisibleAppsLinkagesRequest

A request body you use to add or remove visible apps from a user.

object UserVisibleAppsLinkagesResponse

A response body that contains a list of related resource IDs.

