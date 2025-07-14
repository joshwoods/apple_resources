

- App Store Connect API
-  Delete an Introductory Offer from a Subscription 

Web Service Endpoint

# Delete an Introductory Offer from a Subscription

Delete a specific introductory offer for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptions/{id}/relationships/introductoryOffers
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

SubscriptionIntroductoryOffersLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

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

