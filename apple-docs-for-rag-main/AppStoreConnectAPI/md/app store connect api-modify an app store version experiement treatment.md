

- App Store Connect API
-  Modify an App Store version experiement treatment 

Web Service Endpoint

# Modify an App Store version experiement treatment

Update the name and app icon name for a specific App Store version experiment.

App Store Connect API 1.7+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppStoreVersionExperimentTreatmentUpdateRequest

Content-Type: application/json

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Endpoints

GET /v1/appStoreVersionExperimentTreatments/{id}

GET /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations

POST /v1/appStoreVersionExperimentTreatments

Delete a Treatment for an App Store Version Experiment

Delete metadata that you configured for an App Store Version experiment.

