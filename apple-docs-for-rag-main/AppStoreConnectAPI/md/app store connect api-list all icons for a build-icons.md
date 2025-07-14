

- App Store Connect API
-  List All Icons for a Build 

Web Service Endpoint

# List All Icons for a Build

List all the icons for various platforms delivered with a build.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/builds/{id}/icons
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[buildIcons]`

`[string]`

Possible Values: `name, iconAsset, iconType`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

BuildIconsWithoutIncludesResponse

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

