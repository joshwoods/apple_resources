

- App Store Connect API
-  Delete an App Event Localization 

Web Service Endpoint

# Delete an App Event Localization

Delete localized metadata that you configured for an in-app event.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appEventLocalizations/{id}
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

GET /v1/appEventLocalizations/{id}

GET /v1/appEventLocalizations/{id}/appEventVideoClips

GET /v1/appEventLocalizations/{id}/appEventScreenshots

PATCH /v1/appEventLocalizations/{id}

POST /v1/appEventLocalizations

