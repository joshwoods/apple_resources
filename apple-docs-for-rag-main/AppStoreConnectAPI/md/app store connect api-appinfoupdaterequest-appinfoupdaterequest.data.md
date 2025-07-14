

- App Store Connect API
- AppInfoUpdateRequest
-  AppInfoUpdateRequest.Data 

Object

# AppInfoUpdateRequest.Data

The data element of the request body.

App Store Connect API 1.2+

``` source
object AppInfoUpdateRequest.Data
```

## Properties

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

`relationships`

AppInfoUpdateRequest.Data.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `appInfos`

## Topics

### Objects

object AppInfoUpdateRequest.Data.Relationships

The data and links that describe the relationship between the resources.

