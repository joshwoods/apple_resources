

- App Store Connect API
-  Read Information About the Availability of a Subscription 

Web Service Endpoint

# Read Information About the Availability of a Subscription

Get information about the territory availability for a subscription.

App Store Connect API 2.4+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptions/{id}/subscriptionAvailability
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the in-app purchase resource ID from the List All Subscriptions for a Subscription Group response.

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

App Store Connect API 2.4 release notes

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/subscriptions/6448262369/subscriptionAvailability
```

```
{
  “data”: {
    “type”: “subscriptionAvailabilities”,
    “id”: “6448262369”,
    “attributes”: {
      “availableInNewTerritories”: false
    },
    “relationships”: {
      “availableTerritories”: {
        “links”: {
          “self”: “https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6448262369/relationships/availableTerritories”,
          “related”: “https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6448262369/availableTerritories”
        }
      }
    },
    “links”: {
      “self”: “https://api.appstoreconnect.apple.com/v1/subscriptionAvailabilities/6448262369”
    }
  },
  “links”: {
    “self”: “https://api.appstoreconnect.apple.com/v1/subscriptions/6448262369/subscriptionAvailability”
  }
}

```

## See Also

### Endpoints

Create an Auto-Renewable Subscription

Create an auto-renewable subscription for your app.

Read Subscription Information

Get information about a specific auto-renewable subscription.

Modify an Auto-Renewable Subscription

Update a specific auto-renewable subscription.

Delete a Subscription

Delete a specific auto-renewable subscription that you configured for an app.

List All Localizations for an Auto-Renewable Subscription

Get a list of the subscription localizations for a specific auto-renewable subscription.

List All Introductory Offers for a Subscription

Get a list of introductory offers for a specific auto-renewable subscription.

List All Introductory Offer Resource IDs for an Auto-Renewable Subscription

Get a list of resource IDs representing introductory offers for an auto-renewable subscription.

Delete an Introductory Offer from a Subscription

Delete a specific introductory offer for an auto-renewable subscription.

Read Promoted Purchase Information for a Subscription

Get details about the promoted purchase of an auto-renewable subscription.

List All Offer Codes for a Subscription

Get a list of subscription offer codes for a specific auto-renewable subscription.

List All Promotional Offer Resource IDs for an Auto-Renewable Subscription

Get a list of promotional offers for a specific auto-renewable subscription.

List All Price Points for a Subscription

Get a list of price points for an auto-renewable subscription by territory.

List All Prices for a Subscription

Get a list of prices for an auto-renewable subscription, by territory.

List All Subscription Prices IDs for an Auto-Renewable Subscription

Get a list of resource IDs representing subscription prices for an auto-renewable subscription.

Delete Prices from a Subscription

Delete a scheduled subscription price change for an auto-renewable subscription.

