

- App Store Connect API
-  List Prerelease Versions 

Web Service Endpoint

# List Prerelease Versions

Get a list of prerelease versions for all apps.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/preReleaseVersions
```

## Query Parameters

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[preReleaseVersions]`

`[string]`

Fields to return for included related types.

Possible Values: `version, platform, builds, app`

`filter[app]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[builds.expired]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[builds.processingState]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `PROCESSING, FAILED, INVALID, VALID`

`filter[builds]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[platform]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `IOS, MAC_OS, TV_OS, VISION_OS`

`filter[version]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `builds, app`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`limit[builds]`

`integer`

Number of included related resources to return.

Maximum: `50`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `version, -version`

`filter[builds.version]`

`[string]`

## Response Codes

` 200 ``OK`

PreReleaseVersionsResponse

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

### Getting Prerelease Version Information

Read Prerelease Version Information

Get information about a specific prerelease version.

Read the App Information of a Prerelease Version

Get the app information for a specific prerelease version.

