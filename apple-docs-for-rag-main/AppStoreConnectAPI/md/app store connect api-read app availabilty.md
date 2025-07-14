

- App Store Connect API
-  Read App Availabilty 

Web Service Endpoint

# Read App Availabilty

Get information about your app’s availalbility.

App Store Connect API 3.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v2/appAvailabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appAvailabilities]`

`[string]`

Possible Values: `availableInNewTerritories, territoryAvailabilities`

`fields[territoryAvailabilities]`

`[string]`

Possible Values: `available, releaseDate, preOrderEnabled, preOrderPublishDate, contentStatuses, territory`

`include`

`[string]`

Value: `territoryAvailabilities`

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

## Mentioned in 

App Store Connect API 3.1 release notes

## See Also

### Managing app and territory availability

Read App Availablity Territories

Read the territory availablity for a specific app.

Create an App Pre-Order

Create an app pre-order and set the expected app release date.

Modify the Territory Availabilty for an App Pre-Order

Update the release territories for your app pre-order.

End an App Pre-Order

End the pre-order for your app and release to store immediately.

