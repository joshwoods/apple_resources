

- App Store Connect API
-  Read Device Information 

Web Service Endpoint

# Read Device Information

Get information for a specific device registered to your team.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/devices/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[devices]`

`[string]`

Possible Values: `name, platform, udid, deviceClass, status, model, addedDate`

## Response Codes

` 200 ``OK`

DeviceResponse

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

### Getting Device Information

List Devices

Find and list devices registered to your team.

