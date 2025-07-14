

- App Store Connect API
-  Create an Introductory Offer 

Web Service Endpoint

# Create an Introductory Offer

Create an introductory offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionIntroductoryOffers
```

## HTTP Body

SubscriptionIntroductoryOfferCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionIntroductoryOfferResponse

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

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Modify an Introductory Offer

Update a specific introductory offer for an auto-renewable subscription.

Delete an Introductory Offer for a Subscription

Delete a specific introductory offer for an auto-renewable subscription.

