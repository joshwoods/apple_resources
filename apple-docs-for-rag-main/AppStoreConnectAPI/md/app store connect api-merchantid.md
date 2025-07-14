

- App Store Connect API
-  MerchantId 

Object

# MerchantId

The data structure that represents a merchant ID resource.

App Store Connect API 3.8+

``` source
object MerchantId
```

## Properties

`attributes`

MerchantId.Attributes

Attributes that describe a merchant ID resource.

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the merchant ID resource ID from the List merchant IDs response.

`links`

ResourceLinks

Navigational links that include the self-link.

`relationships`

MerchantId.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `merchantIds`

## Topics

### Dictionaries

object MerchantId.Attributes

Attributes that describe a merchant ID resource.

object MerchantId.Relationships

The relationship you include in the request and those on which you can operate.

## See Also

### Objects

object MerchantIdResponse

A response that contains a single merchant ID resource.

object MerchantIdsResponse

A response that contains a list of merchant ID resources.

object MerchantIdCreateRequest

The request body you use to create a merchant ID.

object MerchantIdUpdateRequest

The request body you use to update a merchant ID.

