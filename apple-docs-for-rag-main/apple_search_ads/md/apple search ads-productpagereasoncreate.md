

- Apple Search Ads
-  ProductPageReasonCreate 

Object

# ProductPageReasonCreate

The ad creative rejection reason based on a product page.

``` source
object ProductPageReasonCreate
```

## Properties

`adamId`

`int64`

 (Required) 

Your unique App Store app identifier.

`assetGenId`

`string`

The unique identifier for an app preview or screenshot.

`comment`

`string`

Custom comments from Apple about the rejection reason.

`countryOrRegion`

`string`

 (Required) 

The App Store geoterritories where you’re promoting your app.

`id`

`int64`

 (Read-only) 

The unique identifier for a creative.

`languageCode`

`string`

 (Required) 

The ISO 639-1 language code appended to the ISO 3166-1 alpha-2 country code, such as `en-US`.

`productPageId`

`string`

 (Required) 

The custom product page identifier associated with the ad creative rejection reason. This field is nullable.

`reasonCode`

`string`

 (Required) 

Contains one of the `RejectionReason` enumerations in the Discussion section below.

`reasonLevel`

`string`

The level at which the system applies the rejection reason. See ReasonLevel for enumerations.

`reasonType`

`string`

 (Required) 

The reason type has a value of `REJECTION_REASON`.

`supplySource`

`string`

 (Required) 

The ad placement associated with the ad creative rejection reason.

## Discussion

Descriptions of reason codes include the following:

`APP_ICON_GRAPHIC_OR_ADULT_THEMED_CONTENT`  
Violent, offensive, sexually explicit, or otherwise inappropriate images aren’t allowed in the app icon.

`APP_ICON_NOT_ELIGIBLE`  
The app icon doesn’t comply with Apple advertising guidelines.

`APP_NAME_LANGUAGE_CONFLICT`  
The language in the app name needs to match the language selected in App Store Connect.

`APP_NAME_GRAPHIC_OR_ADULT_THEMED_CONTENT`  
Violent, offensive, sexually explicit, or otherwise inappropriate wording isn’t allowed in the app name.

`APP_NAME_NOT_ELIGIBLE`  
The app name doesn’t comply with Apple advertising guidelines.

`APP_NOT_ELIGIBLE_AT_THIS_TIME`  
The app isn’t eligible for promotion on the Today tab.

`MIMICS_APP_STORE_TODAY_CARD`  
The phrases *Game of the Day* and *App of the Day* aren’t allowed in the app icon, name, or subtitle.

`PRODUCT_PAGE_OPTIMIZATION_EXPERIMENT_APP_ICON_NOT_ELIGIBLE`  
The app icon from a product page optimization (PPO) experiment doesn’t comply with Apple Advertising guidelines.

`SUBTITLE_GRAPHIC_OR_ADULT_THEMED_CONTENT`  
Violent, offensive, sexually explicit, or otherwise inappropriate wording isn’t allowed in the app subtitle.

`SUBTITLE_LANGUAGE_CONFLICT`  
The language in the app subtitle needs to match the language of the primary locale in App Store Connect.

`SUBTITLE_NOT_ELIGIBLE`  
The app’s subtitle doesn’t comply with Apple Search Ads advertising requirements.

`SUBTITLE_PRICING_OFFERS_OR_RANKING_CLAIMS`  
Pricing, offers, ranking, or other incentivized promotions aren’t allowed in the app subtitle.

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

