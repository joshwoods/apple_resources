

- App Store Connect API
-  Delete a Treatment for an App Store Version Experiment 

Web Service Endpoint

# Delete a Treatment for an App Store Version Experiment

Delete metadata that you configured for an App Store Version experiment.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Endpoints

GET /v1/appStoreVersionExperimentTreatments/{id}

GET /v1/appStoreVersionExperimentTreatments/{id}/appStoreVersionExperimentTreatmentLocalizations

Modify an App Store version experiement treatment

Update the name and app icon name for a specific App Store version experiment.

POST /v1/appStoreVersionExperimentTreatments

