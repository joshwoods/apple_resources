

- App Store Connect API
-  Modify a win-back offer 

Web Service Endpoint

# Modify a win-back offer

Edit details for a specific win-back offer.

App Store Connect API 3.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/winBackOffers/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the `winBackOffers` resource ID from the List win-back offers response.

## HTTP Body

WinBackOfferUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

WinBackOfferResponse

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/winBackOffers/10759170294
{
  "data": {
    "type": "winBackOffers",
    "id": "10778326500",
    "attributes": {
      "promotionIntent": "USE_AUTO_GENERATED_ASSETS",
      "startDate": "2024-07-04",
      "endDate": "2024-07-31"
    }
  }
}        
```

```
"data": {
  "type": "winBackOffers",
  "id": "10778326500",
  "attributes": {
    "referenceName": "6 Months for 3 A",
    "offerId": "6Monthfor3_a",
    "duration": "SIX_MONTHS",
    "offerMode": "PAY_UP_FRONT",
    "periodCount": 1,
    "customerEligibilityPaidSubscriptionTenureInMonths": null,
    "customerEligibilityPaidSubscriptionDurationInMonths": 6,
    "customerEligibilityTimeSinceLastSubscribedInMonths": {
      "minimum": 2,
      "maximum": 24
    },
    "customerEligibilityWaitBetweenOffersInMonths": 2,
    "startDate": "2024-07-04",
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
"links": {
  "self": "https://api.appstoreconnect.apple.com/v1/winBackOffers/10778326500"
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

Create a win-back offer

Create a win-back offer for a specific subscription.

Delete a win-back offer

Remove a win-back offer for a specific subscription.

