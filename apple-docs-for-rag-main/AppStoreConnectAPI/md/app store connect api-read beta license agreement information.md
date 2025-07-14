

- App Store Connect API
-  Read Beta License Agreement Information 

Web Service Endpoint

# Read Beta License Agreement Information

Get a specific beta license agreement.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/betaLicenseAgreements/{id}
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

`fields[betaLicenseAgreements]`

`[string]`

Fields to return for included related types.

Possible Values: `agreementText, app`

`include`

`[string]`

Relationship data to include in the response.

Value: `app`

## Response Codes

` 200 ``OK`

BetaLicenseAgreementResponse

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

### Getting Beta License Agreement Information

List Beta License Agreements

Find and list beta license agreements for all apps.

Read the App Information of a Beta License Agreement

Get the app information for a specific beta license agreement.

