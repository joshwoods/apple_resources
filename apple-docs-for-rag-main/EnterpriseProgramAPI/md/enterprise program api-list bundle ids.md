

- Enterprise Program API
-  List Bundle Ids 

Web Service Endpoint

# List Bundle Ids

Find and list bundle IDs that are registered to your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/bundleIds
```

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

`filter[id]`

`[string]`

`filter[identifier]`

`[string]`

`filter[name]`

`[string]`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS`

`filter[seedId]`

`[string]`

`include`

`[string]`

Possible Values: `bundleIdCapabilities, profiles`

`limit`

`integer`

Maximum: `200`

`limit[bundleIdCapabilities]`

`integer`

Maximum: `50`

`limit[profiles]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `id, -id, identifier, -identifier, name, -name, platform, -platform, seedId, -seedId`

## Response Codes

` 200 ``OK`

BundleIdsResponse

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

## Mentioned in 

Generating Tokens for API Requests

## See Also

### Getting Bundle ID Information

Read BundleId Information

Get information about a specific bundle ID.

