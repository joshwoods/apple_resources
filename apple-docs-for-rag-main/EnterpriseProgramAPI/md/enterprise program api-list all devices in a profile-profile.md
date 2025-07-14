

- Enterprise Program API
-  List All Devices in a Profile 

Web Service Endpoint

# List All Devices in a Profile

Get a list of all devices for a specific provisioning profile.

## URL

``` source
GET https://api.enterprise.developer.apple.com/v1/profiles/{id}/devices
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[devices]`

`[string]`

Possible Values: `addedDate, deviceClass, model, name, platform, status, udid`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

DevicesWithoutIncludesResponse

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

Read the Bundle ID in a Profile

Get the bundle ID information for a specific provisioning profile.

List All Certificates in a Profile

Get a list of all certificates and their data for a specific provisioning profile.

