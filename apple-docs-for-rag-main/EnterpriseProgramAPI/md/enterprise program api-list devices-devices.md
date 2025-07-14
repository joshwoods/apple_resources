

- Enterprise Program API
-  List Devices 

Web Service Endpoint

# List Devices

Find and list devices registered to your team.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/devices
```

## Query Parameters

`fields[devices]`

`[string]`

Possible Values: `addedDate, deviceClass, model, name, platform, status, udid`

`filter[id]`

`[string]`

`filter[name]`

`[string]`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS`

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

Possible Values: `id, -id, name, -name, platform, -platform, status, -status, udid, -udid`

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

