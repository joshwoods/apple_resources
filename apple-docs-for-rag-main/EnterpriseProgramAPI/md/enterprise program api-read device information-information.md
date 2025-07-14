

- Enterprise Program API
-  Read Device Information 

Web Service Endpoint

# Read Device Information

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/devices/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[devices]`

`[string]`

Possible Values: `addedDate, deviceClass, model, name, platform, status, udid`

## Response Codes

` 200 ``OK`

DeviceResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Getting Device Information

List Devices

Find and list devices registered to your team.

