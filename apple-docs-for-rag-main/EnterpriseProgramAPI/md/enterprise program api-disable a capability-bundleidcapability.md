

- Enterprise Program API
-  Disable a Capability 

Web Service Endpoint

# Disable a Capability

Disable a capability for a bundle ID.

## URL

``` source
DELETE https://api.enterprise.developer.apple.com/v1/bundleIdCapabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

\[missing\]

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

### Enabling and Disabling Capabilities

Modify a Capability Configuration

Enable a capability for a bundle ID.

