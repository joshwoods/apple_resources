

- App Store Connect API
- BuildBetaNotificationCreateRequest
- 
  - BuildBetaNotificationCreateRequest
- BuildBetaNotificationCreateRequest.Data
- BuildBetaNotificationCreateRequest.Data.Relationships
- BuildBetaNotificationCreateRequest.Data.Relationships.Build
-  BuildBetaNotificationCreateRequest.Data.Relationships.Build.Data 

Object

# BuildBetaNotificationCreateRequest.Data.Relationships.Build.Data

The type and ID of the resource that you’re relating with the resource you’re creating.

App Store Connect API 1.0+

``` source
object BuildBetaNotificationCreateRequest.Data.Relationships.Build.Data
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The types and IDs of the related data to update.

Value: `builds`

