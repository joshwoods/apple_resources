

- App Store Connect API
-  Create a leaderboard set member localization 

Web Service Endpoint

# Create a leaderboard set member localization

Add a new leaderboard set localization.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetMemberLocalizations
```

## HTTP Body

GameCenterLeaderboardSetMemberLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardSetMemberLocalizationResponse

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

### Managing leaderboard set member localizations

Read leaderboard set member localization information

Get information about leaderboard member set localizations.

Read leaderboard information for a leaderboard set member localization

Get information about a leaderboard for a specific leaderboard set member localization.

Read leaderboard set information for a leaderboard set member localization

Get information about a leaderboard set for a specific leaderboard set member localization.

Modify a leaderboard set member localization

Edit a leaderboard set member localization.

Delete a leaderboard set member localization

Delete a localization that’s associated with a leaderboard set member.

