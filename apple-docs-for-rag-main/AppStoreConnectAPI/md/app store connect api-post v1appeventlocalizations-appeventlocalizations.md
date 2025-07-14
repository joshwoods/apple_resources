

- App Store Connect API
-  POST /v1/appEventLocalizations 

Web Service Endpoint

# POST /v1/appEventLocalizations

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEventLocalizations
```

## HTTP Body

AppEventLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEventLocalizationResponse

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

GET /v1/appEventLocalizations/{id}

GET /v1/appEventLocalizations/{id}/appEventVideoClips

GET /v1/appEventLocalizations/{id}/appEventScreenshots

PATCH /v1/appEventLocalizations/{id}

Delete an App Event Localization

Delete localized metadata that you configured for an in-app event.

