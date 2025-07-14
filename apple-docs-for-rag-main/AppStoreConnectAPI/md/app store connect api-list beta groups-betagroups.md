

- App Store Connect API
-  List Beta Groups 

Web Service Endpoint

# List Beta Groups

Find and list beta groups for all apps.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaGroups
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

`fields[betaRecruitmentCriteria]`

`[string]`

Possible Values: `lastModifiedDate, deviceFamilyOsVersionFilters`

`fields[betaTesters]`

`[string]`

Fields to return for included related types.

Possible Values: `firstName, lastName, email, inviteType, state, apps, betaGroups, builds`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`filter[app]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[builds]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[id]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[isInternalGroup]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[name]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[publicLinkEnabled]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[publicLinkLimitEnabled]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[publicLink]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `app, builds, betaTesters, betaRecruitmentCriteria`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`limit[betaTesters]`

`integer`

Number of included related resources to return.

Maximum: `50`

`limit[builds]`

`integer`

Number of included related resources to return.

Maximum: `1000`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `name, -name, createdDate, -createdDate, publicLinkEnabled, -publicLinkEnabled, publicLinkLimit, -publicLinkLimit`

## Response Codes

` 200 ``OK`

BetaGroupsResponse

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

### Getting Beta Group Information

Read Beta Group Information

Get a specific beta group.

Read the App Information of a Beta Group

Get the app information for a specific beta group.

Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

