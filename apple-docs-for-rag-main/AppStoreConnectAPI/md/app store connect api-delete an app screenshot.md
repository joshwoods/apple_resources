

- App Store Connect API
-  Delete an App Screenshot 

Web Service Endpoint

# Delete an App Screenshot

Delete an app screenshot that is associated with a screenshot set.

App Store Connect API 1.2+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/appScreenshots/{id}
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

### Creating, Modifying, and Deleting Screenshots

Create an App Screenshot

Add a new screenshot to a screenshot set.

Modify an App Screenshot

Commit an app screenshot after uploading it.

