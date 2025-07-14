

- App Store Connect API
-  Read App Information for an Xcode Cloud Product 

Web Service Endpoint

# Read App Information for an Xcode Cloud Product

Get the app in App Store Connect that’s related to an Xcode Cloud product.

App Store Connect API 1.5+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/ciProducts/{id}/app
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Products resource.

## Query Parameters

`fields[appInfos]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `appStoreState, state, appStoreAgeRating, australiaAgeRating, brazilAgeRating, brazilAgeRatingV2, franceAgeRating, koreaAgeRating, kidsAgeBand, app, ageRatingDeclaration, appInfoLocalizations, primaryCategory, primarySubcategoryOne, primarySubcategoryTwo, secondaryCategory, secondarySubcategoryOne, secondarySubcategoryTwo`

`fields[appStoreVersions]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[apps]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[betaAppLocalizations]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `feedbackEmail, marketingUrl, privacyPolicyUrl, tvOsPrivacyPolicy, description, locale, app`

`fields[betaGroups]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `name, createdDate, isInternalGroup, hasAccessToAllBuilds, publicLinkEnabled, publicLinkId, publicLinkLimitEnabled, publicLinkLimit, publicLink, feedbackEnabled, iosBuildsAvailableForAppleSiliconMac, iosBuildsAvailableForAppleVision, app, builds, betaTesters, betaRecruitmentCriteria, betaRecruitmentCriterionCompatibleBuildCheck`

`fields[builds]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[gameCenterEnabledVersions]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `platform, versionString, iconAsset, compatibleVersions, app`

`fields[inAppPurchases]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `referenceName, productId, inAppPurchaseType, state, apps, name, reviewNote, familySharable, contentHosting, inAppPurchaseLocalizations, pricePoints, content, appStoreReviewScreenshot, promotedPurchase, iapPriceSchedule, inAppPurchaseAvailability, images`

`fields[preReleaseVersions]`

`[string]`

Additional fields to include for each Apps resource returned by the response.

Possible Values: `version, platform, builds, app`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `appEncryptionDeclarations, ciProduct, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, endUserLicenseAgreement, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, gameCenterDetail, appStoreVersionExperimentsV2`

`limit[appInfos]`

`integer`

The number of included Apps resources to return if the app info relationship is included.

Maximum: `50`

`limit[appStoreVersions]`

`integer`

The number of included Apps resources to return if the app store versions relationship is included.

Maximum: `50`

`limit[betaAppLocalizations]`

`integer`

The number of included Apps resources to return if the beta app localizations relationship is included.

Maximum: `50`

`limit[betaGroups]`

`integer`

The number of included Apps resources to return if the beta groups relationship is included.

Maximum: `50`

`limit[builds]`

`integer`

The number of included Apps resources to return if the builds relationship is included.

Maximum: `50`

`limit[gameCenterEnabledVersions]`

`integer`

Deprecated 

The number of included Apps resources to return if the Game Center enabled versions relationship is included.

Maximum: `50`

`limit[inAppPurchases]`

`integer`

Deprecated 

The number of included Apps resources to return if the in-app purchases relationship is included.

Maximum: `50`

`limit[preReleaseVersions]`

`integer`

The number of included Apps resources to return if the pre-release versions relationship is included.

Maximum: `50`

`limit[appClips]`

`integer`

Maximum: `50`

`fields[appClips]`

`[string]`

Possible Values: `bundleId, app, appClipDefaultExperiences, appClipAdvancedExperiences`

`fields[reviewSubmissions]`

`[string]`

Possible Values: `platform, submittedDate, state, app, items, appStoreVersionForReview, submittedByActor, lastUpdatedByActor`

`fields[appCustomProductPages]`

`[string]`

Possible Values: `name, url, visible, app, appCustomProductPageVersions`

`fields[appEvents]`

`[string]`

Possible Values: `referenceName, badge, eventState, deepLink, purchaseRequirement, primaryLocale, priority, purpose, territorySchedules, archivedTerritorySchedules, localizations`

`limit[appCustomProductPages]`

`integer`

Maximum: `50`

`limit[appEvents]`

`integer`

Maximum: `50`

`limit[reviewSubmissions]`

`integer`

Maximum: `50`

`fields[betaLicenseAgreements]`

`[string]`

Possible Values: `agreementText, app`

`fields[betaAppReviewDetails]`

`[string]`

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, app`

`fields[ciProducts]`

`[string]`

Possible Values: `name, createdDate, productType, app, bundleId, workflows, primaryRepositories, additionalRepositories, buildRuns`

`fields[endUserLicenseAgreements]`

`[string]`

Possible Values: `agreementText, app, territories`

`fields[subscriptionGracePeriods]`

`[string]`

Possible Values: `optIn, sandboxOptIn, duration, renewalType`

`fields[subscriptionGroups]`

`[string]`

Possible Values: `referenceName, subscriptions, subscriptionGroupLocalizations`

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`limit[subscriptionGroups]`

`integer`

Maximum: `50`

`limit[inAppPurchasesV2]`

`integer`

Maximum: `50`

`limit[promotedPurchases]`

`integer`

Maximum: `50`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, platform, trafficProportion, state, reviewRequired, startDate, endDate, app, latestControlVersion, controlVersions, appStoreVersionExperimentTreatments`

`limit[appStoreVersionExperimentsV2]`

`integer`

Maximum: `50`

`fields[appEncryptionDeclarations]`

`[string]`

Possible Values: `appDescription, createdDate, usesEncryption, exempt, containsProprietaryCryptography, containsThirdPartyCryptography, availableOnFrenchStore, platform, uploadedDate, documentUrl, documentName, documentType, appEncryptionDeclarationState, codeValue, app, builds, appEncryptionDeclarationDocument`

`limit[appEncryptionDeclarations]`

`integer`

Maximum: `50`

`fields[gameCenterDetails]`

`[string]`

Possible Values: `arcadeEnabled, challengeEnabled, app, gameCenterAppVersions, gameCenterGroup, gameCenterLeaderboards, gameCenterLeaderboardSets, gameCenterAchievements, defaultLeaderboard, defaultGroupLeaderboard, achievementReleases, leaderboardReleases, leaderboardSetReleases`

## Response Codes

` 200 ``OK`

AppResponse

`OK`

The request completed successfully.

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

### Getting Xcode Cloud Products

List All Xcode Cloud Products

Get a list of all products you created in Xcode Cloud.

Read Xcode Cloud Product Information

Get information about a specific Xcode Cloud product.

List All Additional Repositories for an Xcode Cloud Product

List all additional Git repositories you associated with an Xcode Cloud product.

List All Xcode Cloud Builds for an Xcode Cloud Product

List all builds Xcode Cloud performed for a specific product.

List All Primary Git Repositories for an Xcode Cloud Product

List all primary Git repositories for a specific Xcode Cloud product.

List All Workflows for an Xcode Cloud Product

List all workflows for a specific Xcode Cloud product.

Read the Xcode Cloud Product for an App

Get the Xcode Cloud product information for an app you build with Xcode Cloud.

