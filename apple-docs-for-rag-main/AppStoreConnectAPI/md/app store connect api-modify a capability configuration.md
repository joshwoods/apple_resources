

- App Store Connect API
-  Modify a Capability Configuration 

Web Service Endpoint

# Modify a Capability Configuration

Update the configuration of a specific capability.

App Store Connect API 1.1+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/bundleIdCapabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

BundleIdCapabilityUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

BundleIdCapabilityResponse

`OK`

Content-Type: application/json

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

` 422 `

ErrorResponse

Content-Type: application/json

