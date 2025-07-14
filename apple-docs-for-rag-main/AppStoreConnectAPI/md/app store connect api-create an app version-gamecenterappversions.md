

- App Store Connect API
-  Create an app version 

Web Service Endpoint

# Create an app version

Add a new Game Center app version.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterAppVersions
```

## HTTP Body

GameCenterAppVersionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterAppVersionResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Creating, editing, and deleting Game Center app versions

Create a compatiblity relationship

Create a relationship between two Game Center app versions.

Modify an app version

Change the state of Game Center enablement for an app version.

Remove a compatilibly version

Remove a compatilible version relationship from an app version.

