

- App Store Connect API
-  Read App Store Version Information for a Default App Clip Experience 

Web Service Endpoint

# Read App Store Version Information for a Default App Clip Experience

Get App Store Version information for a default App Clip experience.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipDefaultExperiences/{id}/releaseWithAppStoreVersion
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the Default App Clip Experiences resource.

## Query Parameters

`fields[appStoreVersionLocalizations]`

`[string]`

Additional fields to include for each App Store Versions resource returned by the response.

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

`fields[appStoreVersions]`

`[string]`

Additional fields to include for each App Store Versions resource returned by the response.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`include`

`[string]`

The relationship data to include in the response.

Possible Values: `app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, alternativeDistributionPackage`

`limit[appStoreVersionLocalizations]`

`integer`

The number of included Default App Clip Experiences resources to return if the App Store version localizations relationship is included.

Maximum: `50`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments, platform, app, latestControlVersion, controlVersions`

`limit[appStoreVersionExperiments]`

`integer`

Deprecated 

Maximum: `50`

`fields[ageRatingDeclarations]`

`[string]`

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

`fields[appStoreVersionSubmissions]`

`[string]`

Value: `appStoreVersion`

`fields[appStoreReviewDetails]`

`[string]`

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, appStoreVersion, appStoreReviewAttachments`

`fields[apps]`

`[string]`

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[routingAppCoverages]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreVersion`

`fields[appClipDefaultExperiences]`

`[string]`

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`fields[appStoreVersionPhasedReleases]`

`[string]`

Possible Values: `phasedReleaseState, startDate, totalPauseDuration, currentDayNumber`

`fields[builds]`

`[string]`

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`limit[appStoreVersionExperimentsV2]`

`integer`

Maximum: `50`

`fields[alternativeDistributionPackages]`

`[string]`

Value: `versions`

`fields[gameCenterAppVersions]`

`[string]`

Possible Values: `enabled, compatibilityVersions, appStoreVersion`

## Response Codes

` 200 ``OK`

AppStoreVersionResponse

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

### Getting Default App Clip Experience Information

Read Default App Clip Experience Information

Get a specific default App Clip experience.

Read the App Store Review Detail for a Default App Clip Experience

Get App Store Review details for a specific default App Clip experience.

Read Localization Information for a Default App Clip Experience

Get localized metadata that appears on the App Clip card for a specific default App Clip experience.

Get the App Store Versions Resource ID for a Default App Clip Experience

Get IDs for App Store Versions related to a default App Clip experience.

