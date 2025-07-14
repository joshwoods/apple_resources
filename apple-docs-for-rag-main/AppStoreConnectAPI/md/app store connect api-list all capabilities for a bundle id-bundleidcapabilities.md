

- App Store Connect API
-  List All Capabilities for a Bundle ID 

Web Service Endpoint

# List All Capabilities for a Bundle ID

Get a list of all capabilities for a specific bundle ID.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/bundleIds/{id}/bundleIdCapabilities
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[bundleIdCapabilities]`

`[string]`

Possible Values: `capabilityType, settings`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

BundleIdCapabilitiesWithoutIncludesResponse

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

Read the App Information of a Bundle ID

List All Profiles for a Bundle ID

Get a list of all profiles for a specific bundle ID.

