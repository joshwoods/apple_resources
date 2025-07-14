

- Enterprise Program API
-  Read BundleId Information 

Web Service Endpoint

# Read BundleId Information

Get information about a specific bundle ID.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/bundleIds/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[bundleIdCapabilities]`

`[string]`

Possible Values: `bundleId, capabilityType, settings`

`fields[bundleIds]`

`[string]`

Possible Values: `bundleIdCapabilities, identifier, name, platform, profiles, seedId`

`fields[profiles]`

`[string]`

Possible Values: `bundleId, certificates, createdDate, devices, expirationDate, name, platform, profileContent, profileState, profileType, uuid`

`include`

`[string]`

Possible Values: `bundleIdCapabilities, profiles`

`limit[bundleIdCapabilities]`

`integer`

Maximum: `50`

`limit[profiles]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

BundleIdResponse

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

## See Also

### Getting Bundle ID Information

List Bundle Ids

Find and list bundle IDs that are registered to your team.

