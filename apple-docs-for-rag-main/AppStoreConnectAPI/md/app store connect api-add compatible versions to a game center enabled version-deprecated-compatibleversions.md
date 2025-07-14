

- App Store Connect API
-  Add Compatible Versions to a Game Center Enabled Version Deprecated

Web Service Endpoint

# Add Compatible Versions to a Game Center Enabled Version

App Store Connect API 1.2–3.0Deprecated

Deprecated

This endpoint is deprecated.

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterEnabledVersionCompatibleVersionsLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Getting and Adding Compatible Versions

Get All Compatible Version IDs for a Game Center Enabled VersionDeprecated

