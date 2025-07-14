

- App Store Connect API
-  List All Certificates in a Profile 

Web Service Endpoint

# List All Certificates in a Profile

Get a list of all certificates and their data for a specific provisioning profile.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/profiles/{id}/certificates
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

`fields[certificates]`

`[string]`

Possible Values: `name, certificateType, displayName, serialNumber, platform, expirationDate, certificateContent, activated`

## Response Codes

` 200 ``OK`

CertificatesWithoutIncludesResponse

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

List All Devices in a Profile

Get a list of all devices for a specific provisioning profile.

