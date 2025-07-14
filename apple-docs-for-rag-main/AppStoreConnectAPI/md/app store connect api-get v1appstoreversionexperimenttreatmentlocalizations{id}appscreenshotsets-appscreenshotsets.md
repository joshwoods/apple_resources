

- App Store Connect API
-  GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets 

Web Service Endpoint

# GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets
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

`filter[appCustomProductPageLocalization]`

`[string]`

`filter[appStoreVersionLocalization]`

`[string]`

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

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Endpoints

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets

POST /v1/appStoreVersionExperimentTreatmentLocalizations

Delete a Treatment Localization for an App Store Version Experiment

Delete localized metatdata that you configured for an App Store Version experiment treatment.

