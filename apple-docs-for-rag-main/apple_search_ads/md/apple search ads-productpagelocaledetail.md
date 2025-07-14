

- Apple Search Ads
-  ProductPageLocaleDetail 

Object

# ProductPageLocaleDetail

The product page locale metadata on App Store Connect.

Search Ads 4.0+

``` source
object ProductPageLocaleDetail
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId` used in your campaign.

`appName`

`string`

The app name on App Store Connect.

`appPreviewDeviceWithAssets`

ProductPageLocaleDetail.AppPreviewDeviceWithAssets

A map between the device and available app preview details for that device.

`deviceClasses`

`string`

The device classes assigned to a custom product page on App Store Connect.

Possible Values: `IPAD, IPHONE`

`language`

`string`

The language associated with the ISO alpha-2 country code, such as `US`.

`languageCode`

`string`

The ISO 639-1 language code appended to the ISO 3166-1 alpha-2 country code, such as `en-US`.

`productPageId`

`string`

A unique string to identify a product page on App Store Connect. For example, `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

`promotionalText`

`string`

Text that appears at the top of the main description of a product page.

`shortDescription`

`string`

Concise, informative text used on a product page to describe an app.

`subTitle`

`string`

A summary of an app on a product page that appears below the name of an app.

## Topics

### Objects

object ProductPageLocaleDetail.AppPreviewDeviceWithAssets

A map of app preview device assets.

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

object ProductPageDetail

The product page metadata.

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

