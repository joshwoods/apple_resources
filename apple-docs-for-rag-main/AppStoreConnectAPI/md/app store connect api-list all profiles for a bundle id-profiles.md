

- App Store Connect API
-  List All Profiles for a Bundle ID 

Web Service Endpoint

# List All Profiles for a Bundle ID

Get a list of all profiles for a specific bundle ID.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/bundleIds/{id}/profiles
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

`fields[profiles]`

`[string]`

Possible Values: `name, platform, profileType, profileState, profileContent, uuid, createdDate, expirationDate, bundleId, devices, certificates`

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

Read the App Information of a Bundle ID

List All Capabilities for a Bundle ID

Get a list of all capabilities for a specific bundle ID.

