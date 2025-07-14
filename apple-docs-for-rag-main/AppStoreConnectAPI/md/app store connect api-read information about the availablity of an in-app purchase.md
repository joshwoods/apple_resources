

- App Store Connect API
-  Read information about the Availablity of an In-App Purchase 

Web Service Endpoint

# Read information about the Availablity of an In-App Purchase

Get information about the territory availablity for an in-app purchase.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the in-app purchase resource ID from the List All In-App Purchases for an App response.

## Query Parameters

`fields[inAppPurchaseAvailabilities]`

`[string]`

Possible Values: `availableInNewTerritories, availableTerritories`

`fields[territories]`

`[string]`

Value: `currency`

`include`

`[string]`

Value: `availableTerritories`

`limit[availableTerritories]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

InAppPurchaseAvailabilityResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593
```

```
  "data" : {
    "type" : "inAppPurchaseAvailabilities",
    "id" : "6447501593",
    "attributes" : {
      "availableInNewTerritories" : false
    },
    "relationships" : {
      "availableTerritories" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593/relationships/availableTerritories",
          "related" : "https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593/availableTerritories"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593"
  }
}
```

## See Also

### Endpoints

List the territory availablity of an in-app purchase

List all the territories where an in-app purchase is available.

Modify the territory availablity of an in-app purchase

Update the territory availablity of a specific in-app purchase.

