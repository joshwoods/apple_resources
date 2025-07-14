

- App Store Connect API
-  Modify the Territory Availabilty for an App Pre-Order 

Web Service Endpoint

# Modify the Territory Availabilty for an App Pre-Order

Update the release territories for your app pre-order.

App Store Connect API 3.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/territoryAvailabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

TerritoryAvailabilityUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

TerritoryAvailabilityResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing app and territory availability

Read App Availabilty

Get information about your app’s availalbility.

Read App Availablity Territories

Read the territory availablity for a specific app.

Create an App Pre-Order

Create an app pre-order and set the expected app release date.

End an App Pre-Order

End the pre-order for your app and release to store immediately.

