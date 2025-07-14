

- App Store Connect API
-  List nominations 

Web Service Endpoint

# List nominations

Get all featuring nominations.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/nominations
```

## Query Parameters

`fields[nominations]`

`[string]`

Possible Values: `name, type, description, createdDate, lastModifiedDate, submittedDate, state, publishStartDate, publishEndDate, deviceFamilies, locales, supplementalMaterialsUris, hasInAppEvents, launchInSelectMarketsFirst, notes, preOrderEnabled, relatedApps, createdByActor, lastModifiedByActor, submittedByActor, inAppEvents, supportedTerritories`

`filter[relatedApps]`

`[string]`

`filter[state]`

`[string]`

 (Required) 

Possible Values: `DRAFT, SUBMITTED, ARCHIVED`

`filter[type]`

`[string]`

Possible Values: `APP_LAUNCH, APP_ENHANCEMENTS, NEW_CONTENT`

`include`

`[string]`

Possible Values: `relatedApps, createdByActor, lastModifiedByActor, submittedByActor, inAppEvents, supportedTerritories`

`limit`

`integer`

Maximum: `200`

`limit[inAppEvents]`

`integer`

Maximum: `50`

`limit[relatedApps]`

`integer`

Maximum: `50`

`limit[supportedTerritories]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `lastModifiedDate, -lastModifiedDate, publishStartDate, -publishStartDate, publishEndDate, -publishEndDate, name, -name, type, -type`

## Response Codes

` 200 ``OK`

csv

`OK`

Content-Type: text/csv

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

## See Also

### Managing nominations

Create a featuring nomination

Tell Apple about your upcoming app or feature.

Read details for a nomination

Get information for a specific featuring nomination.

Modify a nomination

Update a specific featuring nomination.

Delete a featuring nomination

Remove a specific featuring nomination.

