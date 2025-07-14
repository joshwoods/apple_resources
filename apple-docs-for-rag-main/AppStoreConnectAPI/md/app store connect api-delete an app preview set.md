

- App Store Connect API
-  Delete an App Preview Set 

Web Service Endpoint

# Delete an App Preview Set

Delete an app preview set and all of its previews.

App Store Connect API 1.2+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appPreviewSets/{id}
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

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

## See Also

### Creating and Deleting Preview Sets

Create an App Preview Set

Add a new app preview set to an App Store version localization for a specific app preview type and display size.

