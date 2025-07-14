

- App Store Connect API
-  List All App Screenshot Sets for an App Store Version Localization 

Web Service Endpoint

# List All App Screenshot Sets for an App Store Version Localization

List all screenshot sets for a specific localization.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/{id}/appScreenshotSets
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`fields[appScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, appScreenshotSet`

`filter[screenshotDisplayType]`

`[string]`

Possible Values: `APP_IPHONE_67, APP_IPHONE_61, APP_IPHONE_65, APP_IPHONE_58, APP_IPHONE_55, APP_IPHONE_47, APP_IPHONE_40, APP_IPHONE_35, APP_IPAD_PRO_3GEN_129, APP_IPAD_PRO_3GEN_11, APP_IPAD_PRO_129, APP_IPAD_105, APP_IPAD_97, APP_DESKTOP, APP_WATCH_ULTRA, APP_WATCH_SERIES_10, APP_WATCH_SERIES_7, APP_WATCH_SERIES_4, APP_WATCH_SERIES_3, APP_APPLE_TV, APP_APPLE_VISION_PRO, IMESSAGE_APP_IPHONE_67, IMESSAGE_APP_IPHONE_61, IMESSAGE_APP_IPHONE_65, IMESSAGE_APP_IPHONE_58, IMESSAGE_APP_IPHONE_55, IMESSAGE_APP_IPHONE_47, IMESSAGE_APP_IPHONE_40, IMESSAGE_APP_IPAD_PRO_3GEN_129, IMESSAGE_APP_IPAD_PRO_3GEN_11, IMESSAGE_APP_IPAD_PRO_129, IMESSAGE_APP_IPAD_105, IMESSAGE_APP_IPAD_97`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`limit`

`integer`

Maximum: `200`

`limit[appScreenshots]`

`integer`

Maximum: `50`

`filter[appStoreVersionExperimentTreatmentLocalization]`

`[string]`

`filter[appCustomProductPageLocalization]`

`[string]`

`fields[appCustomProductPageLocalizations]`

`[string]`

Possible Values: `locale, promotionalText, appCustomProductPageVersion, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionLocalizations]`

`[string]`

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

## Response Codes

` 200 ``OK`

AppScreenshotSetsResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Getting Information from a Localization

List All App Preview Sets for an App Store Version Localization

List all app preview sets for a specific localization.

