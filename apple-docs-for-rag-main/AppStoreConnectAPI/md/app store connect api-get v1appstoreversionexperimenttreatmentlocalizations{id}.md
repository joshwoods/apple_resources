

- App Store Connect API
-  GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id} 

Web Service Endpoint

# GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatmentLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`include`

`[string]`

Possible Values: `appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`limit[appPreviewSets]`

`integer`

Maximum: `50`

`limit[appScreenshotSets]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentTreatmentLocalizationResponse

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

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets

POST /v1/appStoreVersionExperimentTreatmentLocalizations

Delete a Treatment Localization for an App Store Version Experiment

Delete localized metatdata that you configured for an App Store Version experiment treatment.

