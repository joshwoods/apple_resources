

- Apple Search Ads
-  CountryOrRegion 

Object

# CountryOrRegion

The supported locales of a product page.

Search Ads 4.0+

``` source
object CountryOrRegion
```

## Properties

`countryOrRegion`

`string`

The supported App Store territory of your product page.

`defaultLanguages`

`[`LocaleInfo`]`

The default languages of assets to use for a campaign’s CountryOrRegion.

`supportedLanguages`

`[`LocaleInfo`]`

The supported `languages` and `languageCodes` that you use on your product page.

## Mentioned in 

Apple Search Ads Campaign Management API 2

## Discussion

Countries and regions use ISO alpha-2 country codes. Use the `Get Supported Countries or Regions` endpoint to fetch supported languages ands language codes.

## See Also

### Product Page Request and Response Objects

object LocaleInfo

The supported languages and language codes.

object CountriesOrRegionsListResponse

A container for product page responses.

object MediaAppVideoAsset

The app preview or screenshot asset detail.

object ProductPageLocaleDetail

The product page locale metadata on App Store Connect.

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

