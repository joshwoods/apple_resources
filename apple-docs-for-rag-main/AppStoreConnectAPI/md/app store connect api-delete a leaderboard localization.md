

- App Store Connect API
-  Delete a leaderboard localization 

Web Service Endpoint

# Delete a leaderboard localization

Delete a localization that’s associated with a leaderboard.

App Store Connect API 3.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/{id}
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

## Discussion

### Example Request and Response

- Request
- Response

```
DELETE https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardLocalizations/5a75be8c-225a-4fd4-b51f-d33876c2c79b
```

```
HTTP/1.1 204 No Content
```

## See Also

### Managing leaderboard localizations

List all localizations for a leaderboard

Get a list of localized metadata for a leaderboard.

Read leaderboard localization information

Get information about a leaderboard localization.

Read the image for a leaderboard localization

Get information about the image associated with a leaderboard localization.

Create a leaderboard localization

Add a new leaderboard localization.

Modify a leaderboard localization

Edit a leaderboard localization.

