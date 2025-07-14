

- Apple Search Ads
-  ProductPageDetailWithAssets 

Object

# ProductPageDetailWithAssets

The product page asset metadata.

Search Ads 4.0+

``` source
object ProductPageDetailWithAssets
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId` used in your campaign.

`contentProviderId`

`int64`

A unique identifier of the registered content owner.

`creationTime`

`date-time`

 (Read-only) 

The date and time the object was created.

This field is not modifiable.

`id`

`int64`

A unique string to identify a product page on App Store Connect. For example, `45812c9b-c296-43d3-c6a0-c5a02f74bf6e`.

`isDefault`

`boolean`

Indicates if the custom product page is the default on App Store Connect.

`localization`

`[`CreativeLocalizationWithAssets`]`

Localized metadata used on a product page with app preview.

`modificationTime`

`date-time`

 (Read-only) 

The date and time of the most recent modification of the object.

This field is not modifiable.

`name`

`string`

The name of your custom product page, as input through App Store Connect.

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

object ProductPageDetail

The product page metadata.

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

