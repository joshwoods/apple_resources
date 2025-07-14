

- App Store Connect API
-  WinBackOffersResponse 

Object

# WinBackOffersResponse

A response that contains a list of win-back offer resources.

App Store Connect API 3.6+

``` source
object WinBackOffersResponse
```

## Properties

`data`

`[`WinBackOffer`]`

 (Required) 

`included`

`[`WinBackOfferPrice`]`

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

object WinBackOfferPricesResponse

A response that contains a list of win-back offer price resources.

object WinBackOfferResponse

A response that contains a single win-back offer resource.

object WinBackOfferUpdateRequest

The request body you use to update a win-back offer.

object IntegerRange

Describe the upper and lower integer bound of the attribute.

