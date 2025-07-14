

- App Store Connect API
-  GET /v1/appStoreVersionExperimentTreatments/{id} 

Web Service Endpoint

# GET /v1/appStoreVersionExperimentTreatments/{id}

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appStoreVersionExperimentTreatmentLocalizations]`

`[string]`

Possible Values: `locale, appStoreVersionExperimentTreatment, appScreenshotSets, appPreviewSets`

`fields[appStoreVersionExperimentTreatments]`

`[string]`

Possible Values: `name, appIcon, appIconName, promotedDate, appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`include`

`[string]`

Possible Values: `appStoreVersionExperiment, appStoreVersionExperimentV2, appStoreVersionExperimentTreatmentLocalizations`

`limit[appStoreVersionExperimentTreatmentLocalizations]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppStoreVersionExperimentTreatmentResponse

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

GET /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations

Modify an App Store version experiement treatment

Update the name and app icon name for a specific App Store version experiment.

POST /v1/appStoreVersionExperimentTreatments

Delete a Treatment for an App Store Version Experiment

Delete metadata that you configured for an App Store Version experiment.

