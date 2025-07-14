

- App Store Connect API
-  Create a group 

Web Service Endpoint

# Create a group

Add a new group.

App Store Connect API 3.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/gameCenterGroups
```

## HTTP Body

GameCenterGroupCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

GameCenterGroupResponse

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

### Managing groups

Read group information

List information for all groups.

Read group information for a specific group

Read information for a specific group.

Modify a group

Edit the reference name for a group.

Delete a group

Remove a group.

List the achievements in a group

List achievements information for a specific group.

List Game Center details for a group

Read Game Center detail information for a specific group.

List Game Center leaderboard sets in a group

Read Game Center leaderboard sets information for a specific group.

List Game Center leaderboards for a group

Read Game Center leaderboard information for a specific group.

