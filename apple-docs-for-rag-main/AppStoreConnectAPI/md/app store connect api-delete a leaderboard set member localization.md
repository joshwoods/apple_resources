

- App Store Connect API
-  Delete a leaderboard set member localization 

Web Service Endpoint

# Delete a leaderboard set member localization

Delete a localization that’s associated with a leaderboard set member.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetMemberLocalizations/{id}
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

### Managing leaderboard set member localizations

Read leaderboard set member localization information

Get information about leaderboard member set localizations.

Read leaderboard information for a leaderboard set member localization

Get information about a leaderboard for a specific leaderboard set member localization.

Read leaderboard set information for a leaderboard set member localization

Get information about a leaderboard set for a specific leaderboard set member localization.

Create a leaderboard set member localization

Add a new leaderboard set localization.

Modify a leaderboard set member localization

Edit a leaderboard set member localization.

