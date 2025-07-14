

- App Store Connect API
-  Remove Compatible Versions from a Game Center Enabled Version Deprecated

Web Service Endpoint

# Remove Compatible Versions from a Game Center Enabled Version

App Store Connect API 1.2–3.0Deprecated

Deprecated

This object is deprecated.

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterEnabledVersions/{id}/relationships/compatibleVersions
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

### Removing and Replacing Compatible Versions

Replace All Compatible Versions for a Game Center Enabled VersionDeprecated

