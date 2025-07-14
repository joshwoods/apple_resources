

- App Store Connect API
-  PATCH /v1/appEvents/{id} 

Web Service Endpoint

# PATCH /v1/appEvents/{id}

App Store Connect API 1.7+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appEvents/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppEventUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppEventResponse

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

Read in-app event information

GET /v1/appEvents/{id}/localizations

GET /v1/apps/{id}/appEvents

POST /v1/appEvents

Delete an App Event

Delete an in-app event and its related metadata.

