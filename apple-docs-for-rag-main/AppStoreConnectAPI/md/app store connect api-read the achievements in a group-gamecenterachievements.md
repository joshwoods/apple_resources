

- App Store Connect API
-  Read the achievements in a group 

Web Service Endpoint

# Read the achievements in a group

List all the achievements associated with a specific group.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterGroups/{id}/relationships/gameCenterAchievements
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterGroupGameCenterAchievementsLinkagesResponse

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

## See Also

### Reading and modifying group relationships

Read the leaderboard sets in a group

List all the leaderboard sets associated with a specific group.

Read the leaderboards in a group

List all the leaderboard associated with a specific group.

Edit the achievements associated with a group

Modify the achievements in a specific group.

Edit the leaderboard sets associated with a group

Modify the leaderboard sets in a specific group.

Edit the leaderboard associated with a group

Modify the Game Center leaderboards in a specific group.

