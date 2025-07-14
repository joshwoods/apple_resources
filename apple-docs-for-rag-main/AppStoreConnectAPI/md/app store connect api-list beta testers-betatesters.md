

- App Store Connect API
-  List Beta Testers 

Web Service Endpoint

# List Beta Testers

Find and list beta testers for all apps, builds, and beta groups.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaTesters
```

## Query Parameters

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[betaGroups]`

`[string]`

Fields to return for included related types.

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`fields[betaTesters]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[apps]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[betaGroups]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[builds]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[email]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[firstName]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[inviteType]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `EMAIL, PUBLIC_LINK`

`filter[lastName]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `apps, betaGroups, builds`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`limit[apps]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[betaGroups]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[builds]`

`integer`

Number of included related resources to return.

Maximum: `50`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `firstName, -firstName, lastName, -lastName, email, -email, inviteType, -inviteType, state, -state`

`filter[id]`

`[string]`

## Response Codes

` 200 ``OK`

BetaTestersResponse

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

### Getting Beta Tester Information

Read Beta Tester Information

Get a specific beta tester.

