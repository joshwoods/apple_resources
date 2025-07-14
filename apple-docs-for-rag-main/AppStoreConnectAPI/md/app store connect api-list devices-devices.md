

- App Store Connect API
-  List Devices 

Web Service Endpoint

# List Devices

Find and list devices registered to your team.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/devices
```

## Query Parameters

`fields[devices]`

`[string]`

Possible Values: `name, platform, udid, deviceClass, status, model, addedDate`

`filter[id]`

`[string]`

`filter[name]`

`[string]`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS, UNIVERSAL`

`filter[status]`

`[string]`

Possible Values: `ENABLED, DISABLED`

`filter[udid]`

`[string]`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `name, -name, platform, -platform, udid, -udid, status, -status, id, -id`

## Response Codes

` 200 ``OK`

DevicesResponse

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

### Getting Device Information

Read Device Information

Get information for a specific device registered to your team.

