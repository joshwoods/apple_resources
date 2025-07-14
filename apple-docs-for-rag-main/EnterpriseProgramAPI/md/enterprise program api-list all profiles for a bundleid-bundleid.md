

- Enterprise Program API
-  List All Profiles for a BundleId 

Web Service Endpoint

# List All Profiles for a BundleId

Get a list of all profiles for a specific bundle ID.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/bundleIds/{id}/profiles
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[profiles]`

`[string]`

Possible Values: `bundleId, certificates, createdDate, devices, expirationDate, name, platform, profileContent, profileState, profileType, uuid`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

ProfilesWithoutIncludesResponse

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

### Getting Related Data

List All Bundle Id Capabilities for a BundleId

Get a list of all capabilities for a specific bundle ID.

