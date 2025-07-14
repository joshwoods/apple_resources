

- App Store Connect API
-  GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets 

Web Service Endpoint

# GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets
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

`filter[appCustomProductPageLocalization]`

`[string]`

`filter[appStoreVersionLocalization]`

`[string]`

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

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets

POST /v1/appStoreVersionExperimentTreatmentLocalizations

Delete a Treatment Localization for an App Store Version Experiment

Delete localized metatdata that you configured for an App Store Version experiment treatment.

