

- App Store Connect API
-  Create a Game Center achievement release 

Web Service Endpoint

# Create a Game Center achievement release

Create a release for an achievement and a Game Center detail.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterAchievementReleases
```

## HTTP Body

GameCenterAchievementReleaseCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterAchievementReleaseResponse

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

### Managing Game Center achievement releases

List achievement releases 

Read information about the achievement releases for specific Game Center detail.

Read release information for an achievement

Read the state of an achievement release and related information.

Read Game Center achievement release information

Read the state of a specific achievement release.

Delete a Game Center achievement release

Delete a release of an achievement or Game Center detail.

