

- App Store Connect API
-  List win-back offers 

Web Service Endpoint

# List win-back offers

List all win-back offers for a specific subscription.

App Store Connect API 3.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptions/{id}/winBackOffers
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[winBackOfferPrices]`

`[string]`

Possible Values: `territory, subscriptionPricePoint`

`fields[winBackOffers]`

`[string]`

Possible Values: `referenceName, offerId, duration, offerMode, periodCount, customerEligibilityPaidSubscriptionDurationInMonths, customerEligibilityTimeSinceLastSubscribedInMonths, customerEligibilityWaitBetweenOffersInMonths, startDate, endDate, priority, promotionIntent, prices`

`include`

`[string]`

Value: `prices`

`limit`

`integer`

Maximum: `200`

`limit[prices]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

WinBackOffersResponse

`OK`

The request completed successfully.

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

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
https://api.appstoreconnect.apple.com/v1/subscriptions/6447497832/winBackOffers
```

```
{
  "data": [
    {
      "type": "winBackOffers",
      "id": "10778326500",
      "attributes": {
        "referenceName": "6 Months for 3 A",
        "offerId": "6Monthfor3_a",
        "duration": "SIX_MONTHS",
        "offerMode": "PAY_UP_FRONT",
        "periodCount": 1,
        "customerEligibilityPaidSubscriptionDurationInMonths": 6,
        "customerEligibilityTimeSinceLastSubscribedInMonths": {
          "minimum": 2,
          "maximum": 24
        },
        "customerEligibilityWaitBetweenOffersInMonths": 2,
        "startDate": "2024-07-01",
        "endDate": "2024-07-31",
        "priority": "HIGH",
        "promotionIntent": "NOT_PROMOTED"
      },
      "relationships": {
        "promotion": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/relationships/promotion",
            "related": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/promotion"
          }
        },
        "prices": {
          "links": {
            "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/relationships/prices",
            "related": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/prices"
          }
        }
      },
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/subscriptions/6447497832/winBackOffers?limit=1",
  },
  "meta": {
    "paging": {
      "total": 1,
      "limit": 50
    }
  }
}
```

## See Also

### Endpoints

Creating and configuring win-back offers

Configure win-back offers for your auto-renewable subscriptions with the App Store Connect API.

Read win-back offer information

Read details about a specific win-back offer.

List win-back offer prices

List all prices for specific win-back offers.

Create a win-back offer

Create a win-back offer for a specific subscription.

Modify a win-back offer

Edit details for a specific win-back offer.

Delete a win-back offer

Remove a win-back offer for a specific subscription.

