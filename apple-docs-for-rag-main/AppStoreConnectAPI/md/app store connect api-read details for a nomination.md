

- App Store Connect API
-  Read details for a nomination 

Web Service Endpoint

# Read details for a nomination

Get information for a specific featuring nomination.

App Store Connect API 3.8+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/nominations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the nomination resource ID from the List nominations response.

## Query Parameters

`fields[nominations]`

`[string]`

Possible Values: `name, type, description, createdDate, lastModifiedDate, submittedDate, state, publishStartDate, publishEndDate, deviceFamilies, locales, supplementalMaterialsUris, hasInAppEvents, launchInSelectMarketsFirst, notes, preOrderEnabled, relatedApps, createdByActor, lastModifiedByActor, submittedByActor, inAppEvents, supportedTerritories`

`include`

`[string]`

Possible Values: `relatedApps, createdByActor, lastModifiedByActor, submittedByActor, inAppEvents, supportedTerritories`

`limit[inAppEvents]`

`integer`

Maximum: `50`

`limit[relatedApps]`

`integer`

Maximum: `50`

`limit[supportedTerritories]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

NominationResponse

`OK`

Content-Type: application/json

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Managing nominations

Create a featuring nomination

Tell Apple about your upcoming app or feature.

List nominations

Get all featuring nominations.

Modify a nomination

Update a specific featuring nomination.

Delete a featuring nomination

Remove a specific featuring nomination.

