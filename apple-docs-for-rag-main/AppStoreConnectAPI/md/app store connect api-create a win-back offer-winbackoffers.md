

- App Store Connect API
-  Create a win-back offer 

Web Service Endpoint

# Create a win-back offer

Create a win-back offer for a specific subscription.

App Store Connect API 3.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/winBackOffers
```

## HTTP Body

WinBackOfferCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

WinBackOfferResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Note

Important Use a unique referenceName and offerId that you have not used for a promotional offer, offer code, or introductory offer, when you create your win-back offer.

### Example Request and Response

- Request
- Response

```
POST https://api.appstoreconnect.apple.com/v1/winBackOffers
{
  "data": {
    "type": "winBackOffers",
    "attributes": {
      "referenceName": "6 Months for 3 A",
      "offerId": "6Monthfor3_a",
      "startDate": "2024-07-01",
      "endDate": "2024-07-31",
      "priority": "HIGH",
      "promotionIntent": "USE_AUTO_GENERATED_ASSETS",
      "customerEligibilityPaidSubscriptionDurationInMonths": 6,
      "customerEligibilityTimeSinceLastSubscribedInMonths": {
        "minimum": 2,
        "maximum": 24
      },
      "customerEligibilityWaitBetweenOffersInMonths": 2,
      "duration": "SIX_MONTHS",
      "offerMode": "PAY_UP_FRONT",
      "periodCount": 1
    },
    "relationships": {
      "subscription": {
        "data": {
          "type": "subscriptions",
          "id": "6447497832"
        }
      },
      "prices": {
        "data": [
          {
            "id": "${winbackOfferPrice-0}",
            "type": "winBackOfferPrices"
          },
          {
            "id": "${winbackOfferPrice-1}",
            "type": "winBackOfferPrices"
          }
        ]
      }
    }
  },
  "included": [
    {
      "type": "winBackOfferPrices",
      "id": "${winbackOfferPrice-0}",
      "relationships": {
        "subscriptionPricePoint": {
          "data": {
            "type": "subscriptionPricePoints",
            "id": "eyJzIjoiNjQ0NzQ5NzgzMiIsInQiOiJVU0EiLCJwIjoiMTAxMjcifQ"
          }
        }
      }
    },
    {
      "type": "winBackOfferPrices",
      "id": "${winbackOfferPrice-1}",
      "relationships": {
        "subscriptionPricePoint": {
          "data": {
            "type": "subscriptionPricePoints",
            "id": "eyJzIjoiNjQ0NzQ5NzgzMiIsInQiOiJDQU4iLCJwIjoiMTAxNDIifQ"
          }
        }
      }
    }
  ]
}

```

```
{
  "data": {
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
      "promotionIntent": "USE_AUTO_GENERATED_ASSETS"
    },
    "relationships": {
      "promotion": {
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/relationships/promotion",
          "related": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/promotion"
        }
      },
      "prices": {
        "meta": {
          "paging": {
            "total": 2,
            "limit": 10
          }
        },
        "data": [
          {
            "type": "winBackOfferPrices",
            "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiQ0FOIiwicCI6IjEwMTQyIn0"
          },
          {
            "type": "winBackOfferPrices",
            "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiVVNBIiwicCI6IjEwMTI3In0"
          }
        ],
        "links": {
          "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/relationships/prices",
          "related": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500/prices"
        }
      }
    },
    "links": {
      "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500"
    }
  },
  "included": [
    {
      "type": "winBackOfferPrices",
      "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiQ0FOIiwicCI6IjEwMTQyIn0",
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/winBackOfferPrices/eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiQ0FOIiwicCI6IjEwMTQyIn0"
      }
    },
    {
      "type": "winBackOfferPrices",
      "id": "eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiVVNBIiwicCI6IjEwMTI3In0",
      "links": {
        "self": "https://api.appstoreconnect.apple.com/v1/winBackOfferPrices/eyJvIjoiMTA3NzgzMjY1MDAiLCJ0IjoiVVNBIiwicCI6IjEwMTI3In0"
      }
    }
  ],
  "links": {
    "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers"
  }
}

```

## See Also

### Endpoints

Creating and configuring win-back offers

Configure win-back offers for your auto-renewable subscriptions with the App Store Connect API.

List win-back offers

List all win-back offers for a specific subscription.

Read win-back offer information

Read details about a specific win-back offer.

List win-back offer prices

List all prices for specific win-back offers.

Modify a win-back offer

Edit details for a specific win-back offer.

Delete a win-back offer

Remove a win-back offer for a specific subscription.

