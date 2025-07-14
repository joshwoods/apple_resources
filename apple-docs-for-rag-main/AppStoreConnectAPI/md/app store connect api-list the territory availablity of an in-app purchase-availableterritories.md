

- App Store Connect API
-  List the territory availablity of an in-app purchase 

Web Service Endpoint

# List the territory availablity of an in-app purchase

List all the territories where an in-app purchase is available.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/{id}/availableTerritories
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the in-app purchase resource ID from the List All In-App Purchases for an App response.

## Query Parameters

`fields[territories]`

`[string]`

Value: `currency`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

TerritoriesResponse

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
https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593/availableTerritories
```

```
{
  "data" : [ {
    "type" : "territories",
    "id" : "ISL",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/ISL"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/inAppPurchaseAvailabilities/6447501593/availableTerritories"
  },
  "meta" : {
    "paging" : {
      "total" : 1,
      "limit" : 50
    }
  }
}
```

## See Also

### Endpoints

Read information about the Availablity of an In-App Purchase

Get information about the territory availablity for an in-app purchase.

Modify the territory availablity of an in-app purchase

Update the territory availablity of a specific in-app purchase.

