

- App Store Connect API
-  Enable a Capability 

Web Service Endpoint

# Enable a Capability

Enable a capability for a bundle ID.

App Store Connect API 1.1+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/bundleIdCapabilities
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

## See Also

### Enabling and Disabling Capabilities

Disable a Capability

Disable a capability for a bundle ID.

