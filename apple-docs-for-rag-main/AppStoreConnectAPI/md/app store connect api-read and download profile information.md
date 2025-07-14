

- App Store Connect API
-  Read and Download Profile Information 

Web Service Endpoint

# Read and Download Profile Information

Get information for a specific provisioning profile and download its data.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/profiles/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[certificates]`

`[string]`

Possible Values: `name, certificateType, displayName, serialNumber, platform, expirationDate, certificateContent, activated`

`fields[devices]`

`[string]`

Possible Values: `name, platform, udid, deviceClass, status, model, addedDate`

`fields[profiles]`

`[string]`

Possible Values: `name, platform, profileType, profileState, profileContent, uuid, createdDate, expirationDate, bundleId, devices, certificates`

`include`

`[string]`

Possible Values: `bundleId, devices, certificates`

`fields[bundleIds]`

`[string]`

Possible Values: `name, platform, identifier, seedId, profiles, bundleIdCapabilities, app`

`limit[devices]`

`integer`

Maximum: `50`

`limit[certificates]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

ProfileResponse

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

### Getting Provisioning Profile Information

List and Download Profiles

Find and list provisioning profiles and download their data.

