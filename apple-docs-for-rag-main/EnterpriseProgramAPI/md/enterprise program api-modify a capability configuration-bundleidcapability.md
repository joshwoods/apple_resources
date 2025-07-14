

- Enterprise Program API
-  Modify a Capability Configuration 

Web Service Endpoint

# Modify a Capability Configuration

Enable a capability for a bundle ID.

## URL

``` source
POST https://api.enterprise.developer.apple.com/v1/bundleIdCapabilities
```

## HTTP Body

BundleIdCapabilityCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

BundleIdCapabilityResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Overview

- HTTPBody

## See Also

### Enabling and Disabling Capabilities

Disable a Capability

Disable a capability for a bundle ID.

