

- App Store Connect API
-  Read compatible app versions 

Web Service Endpoint

# Read compatible app versions

List all compatible verisons for an app version.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions/{id}/relationships/compatibilityVersions
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

GameCenterAppVersionCompatibilityVersionsLinkagesResponse

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

### Reading Game Center app versions

Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

Read information for a specific app version

Read the Game Center enablement state and related app version information.

Read the App Store version for an app version

Read the app store version and related information for an app version.

Read compatibility version information

Get compatibility version information for a specific app version.

