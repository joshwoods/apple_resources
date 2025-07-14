

- App Store Connect API
-  WinBackOfferPrice 

Object

# WinBackOfferPrice

The data structure that represents a winback offer price resource.

App Store Connect API 3.6+

``` source
object WinBackOfferPrice
```

## Properties

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`relationships`

WinBackOfferPrice.Relationships

Navigational links to related data and included resource types and IDs.

`type`

`string`

 (Required) 

The resource type.

Value: `winBackOfferPrices`

`links`

ResourceLinks

Navigational links that include the self-link.

## Topics

### Objects

object WinBackOfferPrice.Relationships

The relationships you included in the request and those on which you can operate.

## See Also

### Objects

object WinBackOffer

The data structure that represents a win-back offer resource.

object WinBackOfferCreateRequest

The request body you use to create a winback offer.

object WinBackOfferPriceInlineCreate

The data structure that represents a win-back offer price inline create resource.

object WinBackOfferPricesResponse

A response that contains a list of win-back offer price resources.

object WinBackOfferResponse

A response that contains a single win-back offer resource.

object WinBackOfferUpdateRequest

The request body you use to update a win-back offer.

object WinBackOffersResponse

A response that contains a list of win-back offer resources.

object IntegerRange

Describe the upper and lower integer bound of the attribute.

