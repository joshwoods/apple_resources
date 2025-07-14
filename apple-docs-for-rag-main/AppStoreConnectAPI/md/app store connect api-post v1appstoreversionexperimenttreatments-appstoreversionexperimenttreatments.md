

- App Store Connect API
-  POST /v1/appStoreVersionExperimentTreatments 

Web Service Endpoint

# POST /v1/appStoreVersionExperimentTreatments

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatments
```

## HTTP Body

AppStoreVersionExperimentTreatmentCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionExperimentTreatmentResponse

`Created`

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

Modify an App Store version experiement treatment

Update the name and app icon name for a specific App Store version experiment.

Delete a Treatment for an App Store Version Experiment

Delete metadata that you configured for an App Store Version experiment.

