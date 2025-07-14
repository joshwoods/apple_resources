

- App Store Connect API
-  List All App Store Version Localizations for an App Store Version 

Web Service Endpoint

# List All App Store Version Localizations for an App Store Version

Get a list of localized, version-level information about an app, for all locales.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appStoreVersions/{id}/appStoreVersionLocalizations
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`filter[locale]`

`[string]`

`fields[appScreenshotSets]`

`[string]`

Possible Values: `screenshotDisplayType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appScreenshots`

`fields[appStoreVersions]`

`[string]`

Possible Values: `platform, versionString, appStoreState, appVersionState, copyright, reviewType, releaseType, earliestReleaseDate, downloadable, createdDate, app, ageRatingDeclaration, appStoreVersionLocalizations, build, appStoreVersionPhasedRelease, gameCenterAppVersion, routingAppCoverage, appStoreReviewDetail, appStoreVersionSubmission, appClipDefaultExperience, appStoreVersionExperiments, appStoreVersionExperimentsV2, customerReviews, alternativeDistributionPackage`

`fields[appPreviewSets]`

`[string]`

Possible Values: `previewType, appStoreVersionLocalization, appCustomProductPageLocalization, appStoreVersionExperimentTreatmentLocalization, appPreviews`

`fields[appStoreVersionLocalizations]`

`[string]`

Possible Values: `description, locale, keywords, marketingUrl, promotionalText, supportUrl, whatsNew, appStoreVersion, appScreenshotSets, appPreviewSets`

`limit`

`integer`

Maximum: `200`

`limit[appScreenshotSets]`

`integer`

Maximum: `50`

`limit[appPreviewSets]`

`integer`

Maximum: `50`

`include`

`[string]`

Possible Values: `appStoreVersion, appScreenshotSets, appPreviewSets`

## Response Codes

` 200 ``OK`

AppStoreVersionLocalizationsResponse

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

### Getting Version Localizations

Read App Store Version Localization Information

Read localized version-level information.

