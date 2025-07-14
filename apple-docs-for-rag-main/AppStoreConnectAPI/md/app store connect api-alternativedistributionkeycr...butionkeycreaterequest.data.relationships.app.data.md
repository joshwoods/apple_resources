

- App Store Connect API
- AlternativeDistributionKeyCreateRequest
- 
  - AlternativeDistributionKeyCreateRequest
- AlternativeDistributionKeyCreateRequest.Data
- AlternativeDistributionKeyCreateRequest.Data.Relationships
- AlternativeDistributionKeyCreateRequest.Data.Relationships.App
-  AlternativeDistributionKeyCreateRequest.Data.Relationships.App.Data 

Object

# AlternativeDistributionKeyCreateRequest.Data.Relationships.App.Data

The app that is associated with the alternative distribution key.

App Store Connect API 3.3+

``` source
object AlternativeDistributionKeyCreateRequest.Data.Relationships.App.Data
```

## Properties

`id`

`string`

 (Required) 

This is the Apple app ID for the Marketplace app or your web distribution app. An opaque resource ID that uniquely identifies the resource. Obtain the `apps` ID from the List Apps response.

`type`

`string`

 (Required) 

Value: `apps`

