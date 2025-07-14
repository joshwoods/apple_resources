

- App Store Connect API
-  PATCH /v1/appEventLocalizations/{id} 

Web Service Endpoint

# PATCH /v1/appEventLocalizations/{id}

App Store Connect API 1.7+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appEventLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppEventLocalizationUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppEventLocalizationResponse

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

GET /v1/appEventLocalizations/{id}

GET /v1/appEventLocalizations/{id}/appEventVideoClips

GET /v1/appEventLocalizations/{id}/appEventScreenshots

POST /v1/appEventLocalizations

Delete an App Event Localization

Delete localized metadata that you configured for an in-app event.

