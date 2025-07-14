

- App Store Connect API
-  List availability for an app 

Web Service Endpoint

# List availability for an app

Get a list of availabilities for a specific app.

App Store Connect API 3.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/appAvailabilityV2
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[appAvailabilities]`

`[string]`

Possible Values: `availableInNewTerritories, territoryAvailabilities`

`include`

`[string]`

Value: `territoryAvailabilities`

`fields[territoryAvailabilities]`

`[string]`

Possible Values: `available, releaseDate, preOrderEnabled, preOrderPublishDate, contentStatuses, territory`

`limit[territoryAvailabilities]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppAvailabilityV2Response

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

