

- Enterprise Program API
-  Read and Download Profile Information 

Web Service Endpoint

# Read and Download Profile Information

Get information for a specific provisioning profile and download its data.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/profiles/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[bundleIds]`

`[string]`

Possible Values: `bundleIdCapabilities, identifier, name, platform, profiles, seedId`

`fields[certificates]`

`[string]`

Possible Values: `certificateContent, certificateType, csrContent, displayName, expirationDate, name, passTypeId, platform, serialNumber`

`fields[devices]`

`[string]`

Possible Values: `addedDate, deviceClass, model, name, platform, status, udid`

`fields[profiles]`

`[string]`

Possible Values: `bundleId, certificates, createdDate, devices, expirationDate, name, platform, profileContent, profileState, profileType, uuid`

`include`

`[string]`

Possible Values: `bundleId, certificates, devices`

`limit[certificates]`

`integer`

Maximum: `50`

`limit[devices]`

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

