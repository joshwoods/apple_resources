

- Enterprise Program API
-  Delete a BundleId 

Web Service Endpoint

# Delete a BundleId

Delete a bundle ID that is used for app development.

## URL

``` source
DELETE https://api.enterprise.developer.apple.com/v1/bundleIds/{id}
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

### Modifying and Removing Bundle IDs

Modify a PassTypeId

Update a specific bundle ID’s name.

