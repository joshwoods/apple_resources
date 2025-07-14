

- Enterprise Program API
-  List and Download Profiles 

Web Service Endpoint

# List and Download Profiles

Find and list provisioning profiles and download their data.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/profiles
```

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

`filter[id]`

`[string]`

`filter[name]`

`[string]`

`filter[profileState]`

`[string]`

Possible Values: `ACTIVE, INVALID`

`filter[profileType]`

`[string]`

Possible Values: `IOS_APP_DEVELOPMENT, IOS_APP_STORE, IOS_APP_ADHOC, IOS_APP_INHOUSE, MAC_APP_DEVELOPMENT, MAC_APP_STORE, MAC_APP_DIRECT, TVOS_APP_DEVELOPMENT, TVOS_APP_STORE, TVOS_APP_ADHOC, TVOS_APP_INHOUSE, MAC_CATALYST_APP_DEVELOPMENT, MAC_CATALYST_APP_STORE, MAC_CATALYST_APP_DIRECT`

`include`

`[string]`

Possible Values: `bundleId, certificates, devices`

`limit`

`integer`

Maximum: `200`

`limit[certificates]`

`integer`

Maximum: `50`

`limit[devices]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `id, -id, name, -name, profileState, -profileState, profileType, -profileType`

## Response Codes

` 200 ``OK`

ProfilesResponse

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

## See Also

### Getting Provisioning Profile Information

Read and Download Profile Information

Get information for a specific provisioning profile and download its data.

