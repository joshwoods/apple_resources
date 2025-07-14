

- App Store Connect API
-  Read in-app event information 

Web Service Endpoint

# Read in-app event information

App Store Connect API 1.7+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appEvents/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appEventLocalizations]`

`[string]`

Possible Values: `locale, name, shortDescription, longDescription, appEvent, appEventScreenshots, appEventVideoClips`

`fields[appEvents]`

`[string]`

Possible Values: `referenceName, badge, eventState, deepLink, purchaseRequirement, primaryLocale, priority, purpose, territorySchedules, archivedTerritorySchedules, localizations`

`include`

`[string]`

Value: `localizations`

`limit[localizations]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppEventResponse

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

### Endpoints

GET /v1/appEvents/{id}/localizations

GET /v1/apps/{id}/appEvents

PATCH /v1/appEvents/{id}

POST /v1/appEvents

Delete an App Event

Delete an in-app event and its related metadata.

