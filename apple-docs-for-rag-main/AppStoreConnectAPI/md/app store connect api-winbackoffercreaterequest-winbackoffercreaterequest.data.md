

- App Store Connect API
- WinBackOfferCreateRequest
-  WinBackOfferCreateRequest.Data 

Object

# WinBackOfferCreateRequest.Data

The data element of the request body.

App Store Connect API 3.6+

``` source
object WinBackOfferCreateRequest.Data
```

## Properties

`attributes`

WinBackOfferCreateRequest.Data.Attributes

 (Required) 

The attributes that describes the request that creates a win-back offer resource.

`relationships`

WinBackOfferCreateRequest.Data.Relationships

 (Required) 

The navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `winBackOffers`

## Topics

### Objects

object WinBackOfferCreateRequest.Data.Attributes

Attributes that describe a winback offer resource.

object WinBackOfferCreateRequest.Data.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object WinBackOfferPriceInlineCreate

The data structure that represents a win-back offer price inline create resource.

