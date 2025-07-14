

- App Store Connect API
-  Create an Auto-Renewable Subscription 

Web Service Endpoint

# Create an Auto-Renewable Subscription

Create an auto-renewable subscription for your app.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptions
```

## HTTP Body

SubscriptionCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionResponse

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

## Mentioned in 

Managing auto-renewable subscriptions

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

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

Read Review Screenshot Information for a Subscription

Get information about review screenshot for a specific auto-renewable subscription.

