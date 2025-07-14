

- App Store Connect API
-  Read App Store Version Information 

Web Service Endpoint

# Read App Store Version Information

Get information for a specific app store version.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`limit[appStoreVersionLocalizations]`

`integer`

Number of resources to return.

Maximum: `50`

`include`

`[string]`

Relationship data to include in the response. Note: `ageRatingDeclaration` is deprecated.

Possible Values: `app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, alternativeDistributionPackage`

`fields[appStoreVersions]`

`[string]`

Fields to return for included related types. Note: `ageRatingDeclaration` is deprecated.

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appStoreVersionSubmissions]`

`[string]`

Deprecated 

Fields to return for included related types.

Value: `appStoreVersion`

`fields[builds]`

`[string]`

Fields to return for included related types.

Possible Values: `version, uploadedDate, expirationDate, expired, minOsVersion, lsMinimumSystemVersion, computedMinMacOsVersion, iconAssetToken, processingState, buildAudienceType, usesNonExemptEncryption, preReleaseVersion, individualTesters, betaGroups, betaBuildLocalizations, appEncryptionDeclaration, betaAppReviewSubmission, app, buildBetaDetail, appStoreVersion, icons, buildBundles, perfPowerMetrics, diagnosticSignatures`

`fields[appStoreReviewDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, appStoreVersion, appStoreReviewAttachments`

`fields[ageRatingDeclarations]`

`[string]`

Deprecated 

Deprecated. To get age rating declarations, use Read age rating declaration instead.

Possible Values: `alcoholTobaccoOrDrugUseOrReferences, contests, gamblingAndContests, gambling, gamblingSimulated, kidsAgeBand, lootBox, medicalOrTreatmentInformation, profanityOrCrudeHumor, sexualContentGraphicAndNudity, sexualContentOrNudity, horrorOrFearThemes, matureOrSuggestiveThemes, unrestrictedWebAccess, violenceCartoonOrFantasy, violenceRealisticProlongedGraphicOrSadistic, violenceRealistic, ageRatingOverride, koreaAgeRatingOverride, seventeenPlus`

`fields[appStoreVersionPhasedReleases]`

`[string]`

Fields to return for included related types.

Possible Values: `phasedReleaseState, startDate, totalPauseDuration, currentDayNumber`

`fields[routingAppCoverages]`

`[string]`

Fields to return for included related types.

Possible Values: `fileSize, fileName, sourceFileChecksum, uploadOperations, assetDeliveryState, appStoreVersion`

`fields[appStoreVersionLocalizations]`

`[string]`

Fields to return for included related types.

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

`fields[appClipDefaultExperiences]`

`[string]`

Possible Values: `action, appClip, releaseWithAppStoreVersion, appClipDefaultExperienceLocalizations, appClipAppStoreReviewDetail`

`fields[appStoreVersionExperiments]`

`[string]`

Possible Values: `name, trafficProportion, state, reviewRequired, startDate, endDate, appStoreVersion, appStoreVersionExperimentTreatments, platform, app, latestControlVersion, controlVersions`

`limit[appStoreVersionExperiments]`

`integer`

Deprecated 

Maximum: `50`

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

Request succeeded.

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

## Mentioned in 

App Store Connect API 3.6 release notes

## See Also

### Getting App Store Versions

List All App Store Versions for an App

Get a list of all App Store versions of an app across all platforms.

