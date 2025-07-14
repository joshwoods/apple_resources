

- App Store Connect API
-  Delete a leaderboard set localization 

Web Service Endpoint

# Delete a leaderboard set localization

Delete a localization that’s associated with a leaderboard set.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetLocalizations/{id}
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

### Managing leaderboard set localizations

Read leaderboard set localization information

Get information about a leaderboard set localization.

Read the image associated with a leaderboard set localization

Get information about a leaderboard set image associated with a leaderboard set localization.

Create a leaderboard set localization

Add a new leaderboard set localization.

Modify a leaderboard set localization

Edit a leaderboard set localization.

