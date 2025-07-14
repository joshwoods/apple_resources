

- App Store Connect API
-  WinBackOfferPricesResponse 

Object

# WinBackOfferPricesResponse

A response that contains a list of win-back offer price resources.

App Store Connect API 3.6+

``` source
object WinBackOfferPricesResponse
```

## Properties

`data`

`[`WinBackOfferPrice`]`

 (Required) 

`included`

`[*]`

Possible types: Territory`, `SubscriptionPricePoint

`links`

PagedDocumentLinks

 (Required) 

`meta`

PagingInformation

## See Also

### Objects

object WinBackOffer

The data structure that represents a win-back offer resource.

object WinBackOfferCreateRequest

The request body you use to create a winback offer.

object WinBackOfferPrice

The data structure that represents a winback offer price resource.

object WinBackOfferPriceInlineCreate

The data structure that represents a win-back offer price inline create resource.

object WinBackOfferResponse

A response that contains a single win-back offer resource.

object WinBackOfferUpdateRequest

The request body you use to update a win-back offer.

object WinBackOffersResponse

A response that contains a list of win-back offer resources.

object IntegerRange

Describe the upper and lower integer bound of the attribute.

