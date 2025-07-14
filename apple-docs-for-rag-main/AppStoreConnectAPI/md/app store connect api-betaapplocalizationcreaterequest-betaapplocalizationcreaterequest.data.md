

- App Store Connect API
- BetaAppLocalizationCreateRequest
-  BetaAppLocalizationCreateRequest.Data 

Object

# BetaAppLocalizationCreateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object BetaAppLocalizationCreateRequest.Data
```

## Properties

`attributes`

BetaAppLocalizationCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

BetaAppLocalizationCreateRequest.Data.Relationships

 (Required) 

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `betaAppLocalizations`

## Topics

### Objects

object BetaAppLocalizationCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

object BetaAppLocalizationCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

