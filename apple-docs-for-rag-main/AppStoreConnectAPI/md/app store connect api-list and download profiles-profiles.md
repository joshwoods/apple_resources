

- App Store Connect API
-  List and Download Profiles 

Web Service Endpoint

# List and Download Profiles

Find and list provisioning profiles and download their data.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/profiles
```

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

`filter[id]`

`[string]`

`filter[name]`

`[string]`

`include`

`[string]`

Possible Values: `bundleId, devices, certificates`

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

Possible Values: `name, -name, profileType, -profileType, profileState, -profileState, id, -id`

`fields[bundleIds]`

`[string]`

Possible Values: `name, platform, identifier, seedId, profiles, bundleIdCapabilities, app`

`filter[profileState]`

`[string]`

Possible Values: `ACTIVE, INVALID`

`filter[profileType]`

`[string]`

Possible Values: `IOS_APP_DEVELOPMENT, IOS_APP_STORE, IOS_APP_ADHOC, IOS_APP_INHOUSE, MAC_APP_DEVELOPMENT, MAC_APP_STORE, MAC_APP_DIRECT, TVOS_APP_DEVELOPMENT, TVOS_APP_STORE, TVOS_APP_ADHOC, TVOS_APP_INHOUSE, MAC_CATALYST_APP_DEVELOPMENT, MAC_CATALYST_APP_STORE, MAC_CATALYST_APP_DIRECT`

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

