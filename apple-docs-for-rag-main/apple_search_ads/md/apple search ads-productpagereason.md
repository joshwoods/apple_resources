

- Apple Search Ads
-  ProductPageReason 

Object

# ProductPageReason

The ad creative rejection reason based on a product page.

Search Ads 4.8+

``` source
object ProductPageReason
```

## Properties

`adamId`

`int64`

Your unique App Store app identifier. Use Get a Campaign or Get all Campaigns to obtain your `adamId`.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`assetGenId`

`string`

The unique identifier for an app preview or screenshot.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`comment`

`string`

Custom comments from Apple about the rejection reason.

`countryOrRegion`

`string`

The App Store geoterritories where you’re promoting your app.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`id`

`int64`

 (Read-only) 

The rejection reason identifier.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`languageCode`

`string`

The ISO 639-1 language code appended to the ISO 3166-1 alpha-2 country code, such as `en-US`.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`productPageId`

`string`

The custom product page identifier associated with the ad creative rejection reason. This field is nullable.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`reasonCode`

`string`

Contains one of the `RejectionReason` enumerations in the Discussion section below.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`reasonLevel`

`string`

The level at which the system applies the rejection reason. See ReasonLevel for enumerations.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`reasonType`

`string`

The reason type has a value of `REJECTION_REASON`.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

`supplySource`

`string`

The ad placement associated with the ad creative rejection reason.

You can use the `EQUALS` and `IN` Selector Condition operators with Find Ad Creative Rejection Reasons.

## Mentioned in 

Apple Search Ads Campaign Management API 4

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

## Relationships

### Inherited By

- ProductPageReasonResponse

## See Also

### Ad Rejection Reason Objects

object AppAsset

The app assets associated with an adam ID.

object AppAssetListResponse

The response to a request that returns a list of app assets.

object ProductPageReasonListResponse

The response to a request that returns a list of product page rejection reasons.

object ProductPageReasonResponse

A container for product page reasons.

