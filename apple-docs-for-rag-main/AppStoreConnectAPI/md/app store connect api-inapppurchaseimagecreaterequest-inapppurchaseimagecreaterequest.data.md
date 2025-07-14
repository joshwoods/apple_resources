

- App Store Connect API
- InAppPurchaseImageCreateRequest
-  InAppPurchaseImageCreateRequest.Data 

Object

# InAppPurchaseImageCreateRequest.Data

The request body you use to create a subscription purchase image reservation.

App Store Connect API 3.6+

``` source
object InAppPurchaseImageCreateRequest.Data
```

## Properties

`attributes`

InAppPurchaseImageCreateRequest.Data.Attributes

 (Required) 

The resource’s attributes.

`relationships`

InAppPurchaseImageCreateRequest.Data.Relationships

 (Required) 

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `inAppPurchaseImages`

## Topics

### Objects

object InAppPurchaseImageCreateRequest.Data.Attributes

Attributes that describe a subscription purchase image request resource.

object InAppPurchaseImageCreateRequest.Data.Relationships

The relationships you included in the request and those on which you can operate.

