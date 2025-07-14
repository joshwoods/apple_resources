

- App Store Connect API
-  Edit the achievements associated with a group 

Web Service Endpoint

# Edit the achievements associated with a group

Modify the achievements in a specific group.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/gameCenterGroups/{id}/relationships/gameCenterAchievements
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

GameCenterGroupGameCenterAchievementsLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

## See Also

### Reading and modifying group relationships

Read the achievements in a group

List all the achievements associated with a specific group.

Read the leaderboard sets in a group

List all the leaderboard sets associated with a specific group.

Read the leaderboards in a group

List all the leaderboard associated with a specific group.

Edit the leaderboard sets associated with a group

Modify the leaderboard sets in a specific group.

Edit the leaderboard associated with a group

Modify the Game Center leaderboards in a specific group.

