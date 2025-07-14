

- App Store Connect API
-  Read Beta Group Information 

Web Service Endpoint

# Read Beta Group Information

Get a specific beta group.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaGroups/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

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

`include`

`[string]`

Relationship data to include in the response.

Possible Values: `app, builds, betaTesters, betaRecruitmentCriteria`

`limit[builds]`

`integer`

Number of included related resources to return.

Maximum: `1000`

`limit[betaTesters]`

`integer`

Number of included related resources to return.

Maximum: `50`

`fields[betaRecruitmentCriteria]`

`[string]`

Possible Values: `lastModifiedDate, deviceFamilyOsVersionFilters`

## Response Codes

` 200 ``OK`

BetaGroupResponse

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

### Getting Beta Group Information

List Beta Groups

Find and list beta groups for all apps.

Read the App Information of a Beta Group

Get the app information for a specific beta group.

Read metrics for beta testers in a beta group

Get beta tester usage metrics for a beta group.

Read recruitment criteria for a beta group

Get the recruitment criteria information for a specific beta group.

Read build compatibilty for a beta group

Get the build compatibilty information for a specific beta group.

