

- App Store Connect API
-  List the territory availability of a subscription 

Web Service Endpoint

# List the territory availability of a subscription

List the territory availability and currency of a specific subscription.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/{id}/availableTerritories
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the subscription resource ID from the List All Subscriptions for a Subscription Group response.

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
https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418/availableTerritories?limit=5
```

```
{
  "data" : [ {
    "type" : "territories",
    "id" : "SLV",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/SLV"
    }
  }, {
    "type" : "territories",
    "id" : "BRB",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/BRB"
    }
  }, {
    "type" : "territories",
    "id" : "CYM",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/CYM"
    }
  }, {
    "type" : "territories",
    "id" : "NIC",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/NIC"
    }
  }, {
    "type" : "territories",
    "id" : "NAM",
    "attributes" : {
      "currency" : "USD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/NAM"
    }
  } ],
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418/availableTerritories?limit=5",
    "next" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418/availableTerritories?cursor=BQ.AO4JFxQ&limit=5"
  },
  "meta" : {
    "paging" : {
      "total" : 175,
      "limit" : 5
    }
  }
}
```

## See Also

### Endpoints

Read the availability of a subscription

Get information about the territory availability for a subscription.

Modify the territory availability of a subscription

Update the territory availability of a specific subscription.

