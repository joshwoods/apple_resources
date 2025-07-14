

- App Store Connect API
-  Read Beta App Review Detail Information 

Web Service Endpoint

# Read Beta App Review Detail Information

Get beta app review details for a specific app.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaAppReviewDetails/{id}
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

`fields[betaAppReviewDetails]`

`[string]`

Fields to return for included related types.

Possible Values: `contactFirstName, contactLastName, contactPhone, contactEmail, demoAccountName, demoAccountPassword, demoAccountRequired, notes, app`

`include`

`[string]`

Relationship data to include in the response.

Value: `app`

## Response Codes

` 200 ``OK`

BetaAppReviewDetailResponse

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

### Getting Beta App Review Details

List Beta App Review Details

Find and list beta app review details for all apps.

Read the App Information of a Beta App Review Detail

Get the app information for a specific beta app review details resource.

