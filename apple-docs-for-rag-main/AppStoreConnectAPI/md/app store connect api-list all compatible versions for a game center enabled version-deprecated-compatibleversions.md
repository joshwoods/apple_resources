

- App Store Connect API
-  List All Compatible Versions for a Game Center Enabled Version Deprecated

Web Service Endpoint

# List All Compatible Versions for a Game Center Enabled Version

App Store Connect API 1.2–3.0Deprecated

Deprecated

This endpoint is deprecated.

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/gameCenterEnabledVersions/{id}/compatibleVersions
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[gameCenterEnabledVersions]`

`[string]`

Possible Values: `platform, versionString, iconAsset, compatibleVersions, app`

`filter[app]`

`[string]`

`filter[id]`

`[string]`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[versionString]`

`[string]`

`include`

`[string]`

Possible Values: `compatibleVersions, app`

`limit`

`integer`

Maximum: `200`

`sort`

`[string]`

Possible Values: `versionString, -versionString`

`limit[compatibleVersions]`

`integer`

Deprecated 

Maximum: `50`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

GameCenterEnabledVersionsResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Listing Versions

List All Game Center Enabled Versions for an AppDeprecated

