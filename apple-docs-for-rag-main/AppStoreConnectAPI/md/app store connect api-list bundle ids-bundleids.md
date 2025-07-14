

- App Store Connect API
-  List Bundle IDs 

Web Service Endpoint

# List Bundle IDs

Find and list bundle IDs that are registered to your team.

App Store Connect API 1.1+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/bundleIds
```

## Query Parameters

`fields[bundleIds]`

`[string]`

Possible Values: `name, platform, identifier, seedId, profiles, bundleIdCapabilities, app`

`fields[profiles]`

`[string]`

Possible Values: `name, platform, profileType, profileState, profileContent, uuid, createdDate, expirationDate, bundleId, devices, certificates`

`filter[id]`

`[string]`

`filter[identifier]`

`[string]`

`filter[name]`

`[string]`

`filter[platform]`

`[string]`

Possible Values: `IOS, MAC_OS, UNIVERSAL`

`filter[seedId]`

`[string]`

`include`

`[string]`

Possible Values: `profiles, bundleIdCapabilities, app`

`limit`

`integer`

Maximum: `200`

`limit[profiles]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `name, -name, platform, -platform, identifier, -identifier, seedId, -seedId, id, -id`

`fields[bundleIdCapabilities]`

`[string]`

Possible Values: `capabilityType, settings`

`limit[bundleIdCapabilities]`

`integer`

Maximum: `50`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

## Response Codes

` 200 ``OK`

BundleIdsResponse

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

## See Also

### Getting Bundle ID Information

Read Bundle ID Information

Get information about a specific bundle ID.

