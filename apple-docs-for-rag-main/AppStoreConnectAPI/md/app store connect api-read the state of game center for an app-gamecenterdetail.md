

- App Store Connect API
-  Read the state of Game Center for an app 

Web Service Endpoint

# Read the state of Game Center for an app

Get Game Center detail information for an app.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/gameCenterDetail
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[gameCenterAchievementReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterAchievement`

`fields[gameCenterAchievements]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, points, showBeforeEarned, repeatable, archived, gameCenterDetail, gameCenterGroup, groupAchievement, localizations, releases`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`fields[gameCenterGroups]`

`[string]`

Possible Values: `referenceName, gameCenterDetails, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements`

`fields[gameCenterLeaderboardReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboard`

`fields[gameCenterLeaderboardSetReleases]`

`[string]`

Possible Values: `live, gameCenterDetail, gameCenterLeaderboardSet`

`fields[gameCenterLeaderboardSets]`

`[string]`

Possible Values: `referenceName, vendorIdentifier, gameCenterDetail, gameCenterGroup, groupLeaderboardSet, localizations, gameCenterLeaderboards, releases`

`fields[gameCenterLeaderboards]`

`[string]`

Possible Values: `defaultFormatter, referenceName, vendorIdentifier, submissionType, scoreSortType, scoreRangeStart, scoreRangeEnd, recurrenceStartDate, recurrenceDuration, recurrenceRule, archived, gameCenterDetail, gameCenterGroup, groupLeaderboard, gameCenterLeaderboardSets, localizations, releases`

`include`

`[string]`

Possible Values: `app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

`limit[achievementReleases]`

`integer`

Maximum: `50`

`limit[gameCenterAchievements]`

`integer`

Maximum: `50`

`limit[gameCenterAppVersions]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboardSets]`

`integer`

Maximum: `50`

`limit[gameCenterLeaderboards]`

`integer`

Maximum: `50`

`limit[leaderboardReleases]`

`integer`

Maximum: `50`

`limit[leaderboardSetReleases]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

GameCenterDetailResponse

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

### Reading Game Center details

Read Game Center details

Read a specific Game Center detail and related information.

Read app versions for a Game Center detail

Get a list of app versions for a Game Center detail.

Read the groups in a Game Center detail

Get a list of groups in a Game Center detail.

