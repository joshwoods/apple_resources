

- App Store Connect API
-  Get All Compatible Version IDs for a Game Center Enabled Version Deprecated

Web Service Endpoint

# Get All Compatible Version IDs for a Game Center Enabled Version

App Store Connect API 1.2–3.0Deprecated

Deprecated

This endpoint is deprecated.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterEnabledVersionCompatibleVersionsLinkagesResponse

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

### Getting and Adding Compatible Versions

Add Compatible Versions to a Game Center Enabled VersionDeprecated

