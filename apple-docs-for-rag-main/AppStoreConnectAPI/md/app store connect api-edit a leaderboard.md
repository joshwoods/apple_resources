

- App Store Connect API
-  Edit a leaderboard 

Web Service Endpoint

# Edit a leaderboard

Modify the details of a leaderboard.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboards/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the leaderboard resource ID from the Read leaderboard information response.

## HTTP Body

GameCenterLeaderboardUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

GameCenterLeaderboardResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

### Discussion

Use leaderboard formatters to specify the unit of measurement for a Game Center leaderboard. There is a new required attribute `defaultFormatter` when you use Create a leaderboard, which gives all your localizations the same formatter. You can also optionally use `formatterOverride` to override a specific leaderboard localization when calling Create a leaderboard localization or Modify a leaderboard localization.

Before App Store Connect API version 3.0, formatters were based on localizations and were required for each localization. Legacy leaderboards created before the new addition of the Game Center APIs will not have a `defaultFormatter` value, the value would be `null` in this case. Any localizations created before the new addition of the Game Center APIs will always have a `formatterOverride`.

## See Also

### Creating, modifying, and deleting leaderboards

Create a leaderboard

Add a new leaderboard to your app.

Edit the relationship between a leaderboard and a group leaderboard

Modify the group leadboard to which a leaderboard belongs.

Delete a leaderboard

Delete a leaderboard from your app.

