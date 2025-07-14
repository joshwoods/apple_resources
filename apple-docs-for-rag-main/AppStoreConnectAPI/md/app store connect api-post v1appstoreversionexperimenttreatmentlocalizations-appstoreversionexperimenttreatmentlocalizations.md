

- App Store Connect API
-  POST /v1/appStoreVersionExperimentTreatmentLocalizations 

Web Service Endpoint

# POST /v1/appStoreVersionExperimentTreatmentLocalizations

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionExperimentTreatmentLocalizations
```

## HTTP Body

AppStoreVersionExperimentTreatmentLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionExperimentTreatmentLocalizationResponse

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

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appScreenshotSets

GET /v1/appStoreVersionExperimentTreatmentLocalizations/{id}/appPreviewSets

Delete a Treatment Localization for an App Store Version Experiment

Delete localized metatdata that you configured for an App Store Version experiment treatment.

