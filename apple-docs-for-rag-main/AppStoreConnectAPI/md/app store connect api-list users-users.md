

- App Store Connect API
-  List Users 

Web Service Endpoint

# List Users

Get a list of the users on your team.

App Store Connect API 1.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/users
```

## Query Parameters

`fields[apps]`

`[string]`

Fields to return for included related types.

Possible Values: `name, bundleId, sku, primaryLocale, isOrEverWasMadeForKids, subscriptionStatusUrl, subscriptionStatusUrlVersion, subscriptionStatusUrlForSandbox, subscriptionStatusUrlVersionForSandbox, contentRightsDeclaration, streamlinedPurchasingEnabled, appEncryptionDeclarations, ciProduct, betaTesters, betaGroups, appStoreVersions, preReleaseVersions, betaAppLocalizations, builds, betaLicenseAgreement, betaAppReviewDetail, appInfos, appClips, appPricePoints, endUserLicenseAgreement, appPriceSchedule, appAvailabilityV2, inAppPurchases, subscriptionGroups, gameCenterEnabledVersions, perfPowerMetrics, appCustomProductPages, inAppPurchasesV2, promotedPurchases, appEvents, reviewSubmissions, subscriptionGracePeriod, customerReviews, gameCenterDetail, appStoreVersionExperimentsV2, alternativeDistributionKey, analyticsReportRequests, marketplaceSearchDetail`

`fields[users]`

`[string]`

Fields to return for included related types.

Possible Values: `username, firstName, lastName, roles, allAppsVisible, provisioningAllowed, visibleApps`

`include`

`[string]`

Relationship data to include in the response.

Value: `visibleApps`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

`sort`

`[string]`

Attributes by which to sort.

Possible Values: `username, -username, lastName, -lastName`

`filter[roles]`

`[string]`

Attributes, relationships, and IDs by which to filter.

Possible Values: `ADMIN, FINANCE, ACCOUNT_HOLDER, SALES, MARKETING, APP_MANAGER, DEVELOPER, ACCESS_TO_REPORTS, CUSTOMER_SUPPORT, CREATE_APPS, CLOUD_MANAGED_DEVELOPER_ID, CLOUD_MANAGED_APP_DISTRIBUTION, GENERATE_INDIVIDUAL_KEYS`

`filter[visibleApps]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`filter[username]`

`[string]`

Attributes, relationships, and IDs by which to filter.

`limit[visibleApps]`

`integer`

Number of included related resources to return.

Maximum: `50`

## Response Codes

` 200 ``OK`

UsersResponse

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

### Getting User Information

Read User Information

Get information about a user on your team, such as name, roles, and app visibility.

