

- App Store Connect API
-  Delete an App Event Screenshot 

Web Service Endpoint

# Delete an App Event Screenshot

Delete a specific screenshot from an in-app event.

App Store Connect API 1.7+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appEventScreenshots/{id}
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

List the images for an in-app event

PATCH /v1/appEventScreenshots/{id}

POST /v1/appEventScreenshots

