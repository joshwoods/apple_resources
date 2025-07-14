

- App Store Connect API
-  Delete a Bundle ID 

Web Service Endpoint

# Delete a Bundle ID

App Store Connect API 1.1+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/bundleIds/{id}
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

## Discussion

You can only delete bundle IDs that are used for development. You can’t delete bundle IDs that are being used by an app in App Store Connect.

## See Also

### Modifying and Removing Bundle IDs

Modify a Bundle ID

Update a specific bundle ID’s name.

