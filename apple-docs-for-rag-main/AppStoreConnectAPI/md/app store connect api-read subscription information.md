

- App Store Connect API
-  Read Subscription Information 

Web Service Endpoint

# Read Subscription Information

Get information about a specific auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptions/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`fields[subscriptionIntroductoryOffers]`

`[string]`

Possible Values: `startDate, endDate, duration, offerMode, numberOfPeriods, subscription, territory, subscriptionPricePoint`

`fields[subscriptionLocalizations]`

`[string]`

Possible Values: `name, locale, description, state, subscription`

`fields[subscriptionOfferCodes]`

`[string]`

Possible Values: `name, customerEligibilities, offerEligibility, duration, offerMode, numberOfPeriods, totalNumberOfCodes, active, subscription, oneTimeUseCodes, customCodes, prices`

`fields[subscriptionPrices]`

`[string]`

Possible Values: `startDate, preserved, territory, subscriptionPricePoint`

`fields[subscriptions]`

`[string]`

Possible Values: `name, productId, familySharable, state, subscriptionPeriod, reviewNote, groupLevel, subscriptionLocalizations, appStoreReviewScreenshot, group, introductoryOffers, promotionalOffers, offerCodes, prices, pricePoints, promotedPurchase, subscriptionAvailability, winBackOffers, images`

`include`

`[string]`

Possible Values: `subscriptionLocalizations, appStoreReviewScreenshot, group, introductoryOffers, promotionalOffers, offerCodes, prices, promotedPurchase, subscriptionAvailability, winBackOffers, images`

`limit[introductoryOffers]`

`integer`

Maximum: `50`

`limit[offerCodes]`

`integer`

Maximum: `50`

`limit[prices]`

`integer`

Maximum: `50`

`limit[subscriptionLocalizations]`

`integer`

Maximum: `50`

`fields[subscriptionPromotionalOffers]`

`[string]`

Possible Values: `name, offerCode, duration, offerMode, numberOfPeriods, subscription, prices`

`fields[subscriptionAppStoreReviewScreenshots]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, imageAsset, assetToken, assetType, uploadOperations, assetDeliveryState, subscription`

`limit[promotionalOffers]`

`integer`

Maximum: `50`

`fields[subscriptionAvailabilities]`

`[string]`

Possible Values: `availableInNewTerritories, availableTerritories`

`fields[subscriptionImages]`

`[string]`

Possible Values: `fileSize, fileName, sourceFileChecksum, assetToken, imageAsset, uploadOperations, state, subscription`

`fields[winBackOffers]`

`[string]`

Possible Values: `referenceName, offerId, duration, offerMode, periodCount, customerEligibilityPaidSubscriptionDurationInMonths, customerEligibilityTimeSinceLastSubscribedInMonths, customerEligibilityWaitBetweenOffersInMonths, startDate, endDate, priority, promotionIntent, prices`

`limit[images]`

`integer`

Maximum: `50`

`limit[winBackOffers]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

SubscriptionResponse

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

## See Also

### Endpoints

Create an Auto-Renewable Subscription

Create an auto-renewable subscription for your app.

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

