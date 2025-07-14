

- App Store Connect API
- BetaTesterCreateRequest
-  BetaTesterCreateRequest.Data 

Object

# BetaTesterCreateRequest.Data

The data element of the request body.

App Store Connect API 1.0+

``` source
object BetaTesterCreateRequest.Data
```

## Properties

`attributes`

BetaTesterCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

BetaTesterCreateRequest.Data.Relationships

The types and IDs of the related data to update.

`type`

`string`

 (Required) 

The resource type.

Value: `betaTesters`

## Topics

### Objects

object BetaTesterCreateRequest.Data.Attributes

Attributes that you set that describe the new resource.

object BetaTesterCreateRequest.Data.Relationships

The relationships to other resources that you can set with this request.

