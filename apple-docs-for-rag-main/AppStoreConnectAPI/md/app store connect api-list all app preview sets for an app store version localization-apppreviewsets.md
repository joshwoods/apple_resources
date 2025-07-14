

- App Store Connect API
-  List All App Preview Sets for an App Store Version Localization 

Web Service Endpoint

# List All App Preview Sets for an App Store Version Localization

List all app preview sets for a specific localization.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionLocalizations/{id}/appPreviewSets
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appPreviews]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, previewFrameTimeCode, mimeType, videoUrl, previewFrameImage, previewImage, uploadOperations, assetDeliveryState, videoDeliveryState, appPreviewSet`

`filter[previewType]`

`[string]`

Possible Values: `IPHONE_67, IPHONE_61, IPHONE_65, IPHONE_58, IPHONE_55, IPHONE_47, IPHONE_40, IPHONE_35, IPAD_PRO_3GEN_129, IPAD_PRO_3GEN_11, IPAD_PRO_129, IPAD_105, IPAD_97, DESKTOP, APPLE_TV, APPLE_VISION_PRO`

`include`

`[string]`

Possible Values: `appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`limit`

`integer`

Maximum: `200`

`limit[appPreviews]`

`integer`

Maximum: `50`

`filter[appCustomProductPageLocalization]`

`[string]`

`filter[appStoreVersionExperimentTreatmentLocalization]`

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

AppPreviewSetsResponse

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

List All App Screenshot Sets for an App Store Version Localization

List all screenshot sets for a specific localization.

