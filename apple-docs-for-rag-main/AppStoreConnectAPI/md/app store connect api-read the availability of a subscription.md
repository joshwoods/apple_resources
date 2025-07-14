

- App Store Connect API
-  Read the availability of a subscription 

Web Service Endpoint

# Read the availability of a subscription

Get information about the territory availability for a subscription.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the subscription resource ID from the List All Subscriptions for a Subscription Group response.

## Query Parameters

`fields[subscriptionAvailabilities]`

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

SubscriptionAvailabilityResponse

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

App Store Connect API 3.7 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418
```

```
{
  "data" : {
    "type" : "subscriptionAvailabilities",
    "id" : "6447589418",
    "attributes" : {
      "availableInNewTerritories" : false
    },
    "relationships" : {
      "availableTerritories" : {
        "links" : {
          "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418/relationships/availableTerritories",
          "related" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418/availableTerritories"
        }
      }
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6447589418"
  }
}
```

## See Also

### Endpoints

List the territory availability of a subscription

List the territory availability and currency of a specific subscription.

Modify the territory availability of a subscription

Update the territory availability of a specific subscription.

