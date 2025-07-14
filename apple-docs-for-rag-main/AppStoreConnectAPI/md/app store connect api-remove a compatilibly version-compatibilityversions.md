

- App Store Connect API
-  Remove a compatilibly version 

Web Service Endpoint

# Remove a compatilibly version

Remove a compatilible version relationship from an app version.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterAppVersionCompatibilityVersionsLinkagesRequest

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

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, editing, and deleting Game Center app versions

Create an app version

Add a new Game Center app version.

Create a compatiblity relationship

Create a relationship between two Game Center app versions.

Modify an app version

Change the state of Game Center enablement for an app version.

