

- App Store Connect API
-  POST /v1/appEvents 

Web Service Endpoint

# POST /v1/appEvents

App Store Connect API 1.7+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appEvents
```

## HTTP Body

AppEventCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppEventResponse

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

Read in-app event information

GET /v1/appEvents/{id}/localizations

GET /v1/apps/{id}/appEvents

PATCH /v1/appEvents/{id}

Delete an App Event

Delete an in-app event and its related metadata.

