

- App Store Connect API
-  List All Subscriptions for a Subscription Group 

Web Service Endpoint

# List All Subscriptions for a Subscription Group

Get a list of all auto-renewable subscriptions in a subscription group.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionGroups/{id}/subscriptions
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[promotedPurchases]`

`[string]`

Possible Values: `visibleForAllUsers, enabled, state, inAppPurchaseV2, subscription`

`fields[subscriptionGroups]`

`[string]`

Possible Values: `referenceName, subscriptions, subscriptionGroupLocalizations`

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

`filter[name]`

`[string]`

`filter[productId]`

`[string]`

`filter[state]`

`[string]`

Possible Values: `MISSING_METADATA, READY_TO_SUBMIT, WAITING_FOR_REVIEW, IN_REVIEW, DEVELOPER_ACTION_NEEDED, PENDING_BINARY_APPROVAL, APPROVED, DEVELOPER_REMOVED_FROM_SALE, REMOVED_FROM_SALE, REJECTED`

`include`

`[string]`

Possible Values: `subscriptionLocalizations, appStoreReviewScreenshot, group, introductoryOffers, promotionalOffers, offerCodes, prices, promotedPurchase, subscriptionAvailability, winBackOffers, images`

`limit`

`integer`

Maximum: `200`

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

`sort`

`[string]`

Possible Values: `name, -name`

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

SubscriptionsResponse

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

Create a Subscription Group

Create a subscription group for an app.

List All Subscription Groups for an App

Get a list of subscription groups for a specific app.

Read Subscription Group Information

Get the details of a specific subscription group.

Modify a Subscription Group

Update the reference name for a specific subscription group.

Delete a Subscription Group

Delete a specific empty subscription group.

List All Subscription Group Localizations

Get a list of all localized metadata for a specific subscription group.

