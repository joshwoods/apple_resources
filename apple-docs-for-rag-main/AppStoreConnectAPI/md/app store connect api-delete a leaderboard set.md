

- App Store Connect API
-  Delete a leaderboard set 

Web Service Endpoint

# Delete a leaderboard set

Delete a specifc leaderboard set.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSets/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Creating, editing, and deleting leaderboard sets

Create a leaderboard set

Add a new leaderboard set to your app.

Create a relationship between a leaderboard and a leaderboard set

Add a leaderboard to a leaderboard set.

Edit a leaderboard set

Modify the metadata for a leaderboard set.

Modify the leaderboards in leaderboard set

Edit the positions of leaderboards in an existing leaderboard set.

Edit the releationship between a leaderboard and a group leaderboard

Modify the group leaderboards in a leaderboard set.

Delete the relationship between a leaderboard and a leaderboard set

Remove a leaderboard from a leaderboard set.

