

- App Store Connect API
- BetaGroupCreateRequest
-  BetaGroupCreateRequest.Data 

Object

# BetaGroupCreateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object BetaGroupCreateRequest.Data
```

## Properties

`attributes`

BetaGroupCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

BetaGroupCreateRequest.Data.Relationships

 (Required) 

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaGroups`

## Topics

### Objects

object BetaGroupCreateRequest.Data.Attributes

Attributes that you set that describe the new beta group resource.

object BetaGroupCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

