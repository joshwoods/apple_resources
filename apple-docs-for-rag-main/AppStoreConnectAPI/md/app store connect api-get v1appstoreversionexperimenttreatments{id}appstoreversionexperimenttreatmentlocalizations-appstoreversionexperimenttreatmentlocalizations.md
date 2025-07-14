

- App Store Connect API
-  GET /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations 

Web Service Endpoint

# GET /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations
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

`filter[locale]`

`[string]`

`include`

`[string]`

Possible Values: `appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`limit`

`integer`

Maximum: `200`

`limit[appPreviewSets]`

`integer`

Maximum: `50`

`limit[appScreenshotSets]`

`integer`

Maximum: `50`

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentTreatmentLocalizationsResponse

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

GET /v1/appStoreVersionExperimentTreatments/{id}

Modify an App Store version experiement treatment

Update the name and app icon name for a specific App Store version experiment.

POST /v1/appStoreVersionExperimentTreatments

Delete a Treatment for an App Store Version Experiment

Delete metadata that you configured for an App Store Version experiment.

