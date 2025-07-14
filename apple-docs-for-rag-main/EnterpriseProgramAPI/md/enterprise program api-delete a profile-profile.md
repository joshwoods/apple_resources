

- Enterprise Program API
-  Delete a Profile 

Web Service Endpoint

# Delete a Profile

Delete a provisioning profile that is used for app development or distribution.

## URL

``` source
DELETE https://api.enterprise.developer.apple.com/v1/profiles/{id}
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

You can delete provisioning profiles, and may wish to do so if they are expiring or obsolete.

## See Also

### Creating and Deleting Provisioning Profiles

Create a Profile

Create a new provisioning profile.

