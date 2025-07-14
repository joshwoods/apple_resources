

- Device Management
- ManagedApplicationListResponse
- ManagedApplicationListResponse.ManagedApplicationList
-  ManagedApplicationListResponse.ManagedApplicationList.ANY app identifier 

Device Management Command

# ManagedApplicationListResponse.ManagedApplicationList.ANY app identifier

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationListResponse.ManagedApplicationList.ANY app identifier
```

## Properties

`ExternalVersionIdentifier`

`integer`

 (Required) 

`HasConfiguration`

`boolean`

 (Required) 

`HasFeedback`

`boolean`

 (Required) 

`IsValidated`

`boolean`

 (Required) 

`ManagementFlags`

`integer`

 (Required) 

`Status`

`string`

 (Required) 

Possible Values: `Queued, NeedsRedemption, Redeeming, Prompting, PromptingForLogin, ValidatingPurchase, PromptingForUpdate, PromptingForUpdateLogin, PromptingForManagement, ValidatingUpdate, Updating, Installing, Managed, ManagedButUninstalled, Unknown, UserInstalledApp, UserRejected, UpdateRejected, ManagementRejected, Failed`

`UnusedRedemptionCode`

`string`

 (Required) 

