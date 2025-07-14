

- App Store Connect API
-  Create a leaderboard set localization 

Web Service Endpoint

# Create a leaderboard set localization

Add a new leaderboard set localization.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetLocalizations
```

## HTTP Body

GameCenterLeaderboardSetLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardSetLocalizationResponse

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

### Managing leaderboard set localizations

Read leaderboard set localization information

Get information about a leaderboard set localization.

Read the image associated with a leaderboard set localization

Get information about a leaderboard set image associated with a leaderboard set localization.

Modify a leaderboard set localization

Edit a leaderboard set localization.

Delete a leaderboard set localization

Delete a localization that’s associated with a leaderboard set.

