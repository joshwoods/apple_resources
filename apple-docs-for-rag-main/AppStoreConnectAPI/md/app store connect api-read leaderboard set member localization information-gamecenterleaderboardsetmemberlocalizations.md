

- App Store Connect API
-  Read leaderboard set member localization information 

Web Service Endpoint

# Read leaderboard set member localization information

Get information about leaderboard member set localizations.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterLeaderboardSetMemberLocalizations
```

## Query Parameters

`fields[gameCenterLeaderboardSetMemberLocalizations]`

`[string]`

Possible Values: `name, locale, gameCenterLeaderboardSet, gameCenterLeaderboard`

`fields[gameCenterLeaderboardSets]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`filter[gameCenterLeaderboardSet]`

`[string]`

 (Required) 

`filter[gameCenterLeaderboard]`

`[string]`

 (Required) 

`include`

`[string]`

Possible Values: `gameCenterLeaderboardSet, gameCenterLeaderboard`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

GameCenterLeaderboardSetMemberLocalizationsResponse

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

## See Also

### Managing leaderboard set member localizations

Read leaderboard information for a leaderboard set member localization

Get information about a leaderboard for a specific leaderboard set member localization.

Read leaderboard set information for a leaderboard set member localization

Get information about a leaderboard set for a specific leaderboard set member localization.

Create a leaderboard set member localization

Add a new leaderboard set localization.

Modify a leaderboard set member localization

Edit a leaderboard set member localization.

Delete a leaderboard set member localization

Delete a localization that’s associated with a leaderboard set member.

