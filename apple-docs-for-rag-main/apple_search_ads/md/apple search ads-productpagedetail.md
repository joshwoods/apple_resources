

- Apple Search Ads
-  ProductPageDetail 

Object

# ProductPageDetail

The product page metadata.

Search Ads 4.0+

``` source
object ProductPageDetail
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId` used in your campaign.

`creationTime`

`date-time`

 (Read-only) 

The date and time the object was created.

This field is not modifiable.

`deepLink`

`string`

 (Read-only) 

The deep link set up in your custom product page metadata on App Store Connect.

Deep links are available on iOS 18 and later for Today tab and search results ad variations, and iPadOS 18 and later for search results ad variations.

Note that deep links are not available for ads with demographic targeting (age or gender).

This field is not modifiable.

`id`

`string`

A unique string to identify a product page on App Store Connect. For example, `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

This field is not modifiable.

`name`

`string`

The name of your custom product page on App Store Connect.

`state`

`string`

The system state of the custom product page that indicates whether the page is visible or not.

Possible Values: `HIDDEN, VISIBLE`

## Mentioned in 

Apple Search Ads Campaign Management API 5

## See Also

### Product Page Request and Response Objects

object LocaleInfo

The supported languages and language codes.

object CountryOrRegion

The supported locales of a product page.

object CountriesOrRegionsListResponse

A container for product page responses.

object MediaAppVideoAsset

The app preview or screenshot asset detail.

object ProductPageLocaleDetail

The product page locale metadata on App Store Connect.

object ProductPageDetailWithAssets

The product page asset metadata.

object ProductPageLocaleDetailListResponse

A container for product page responses.

object ProductPageDetailResponse

A container for product page responses.

object ProductPageDetailWithAssetInfoResponse

A container for product page responses.

object ProductPageDetailListResponse

A container for product page responses.

object ProductPageReasonCreate

The ad creative rejection reason based on a product page.

