

- App Store Connect API
-  Delete an App Event 

Web Service Endpoint

# Delete an App Event

Delete an in-app event and its related metadata.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appEvents/{id}
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

Read in-app event information

GET /v1/appEvents/{id}/localizations

GET /v1/apps/{id}/appEvents

PATCH /v1/appEvents/{id}

POST /v1/appEvents

