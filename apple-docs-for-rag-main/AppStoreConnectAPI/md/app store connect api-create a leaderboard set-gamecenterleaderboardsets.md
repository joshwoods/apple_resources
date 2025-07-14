

- App Store Connect API
-  Create a leaderboard set 

Web Service Endpoint

# Create a leaderboard set

Add a new leaderboard set to your app.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSets
```

## HTTP Body

GameCenterLeaderboardSetCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterLeaderboardSetResponse

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

### Creating, editing, and deleting leaderboard sets

Create a relationship between a leaderboard and a leaderboard set

Add a leaderboard to a leaderboard set.

Edit a leaderboard set

Modify the metadata for a leaderboard set.

Modify the leaderboards in leaderboard set

Edit the positions of leaderboards in an existing leaderboard set.

Edit the releationship between a leaderboard and a group leaderboard

Modify the group leaderboards in a leaderboard set.

Delete a leaderboard set

Delete a specifc leaderboard set.

Delete the relationship between a leaderboard and a leaderboard set

Remove a leaderboard from a leaderboard set.

