

- App Store Connect API
-  Read Subscription Group Information 

Web Service Endpoint

# Read Subscription Group Information

Get the details of a specific subscription group.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionGroups/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionGroupLocalizations]`

`[string]`

Possible Values: `name, customAppName, locale, state, subscriptionGroup`

`fields[subscriptionGroups]`

`[string]`

Possible Values: `referenceName, subscriptions, subscriptionGroupLocalizations`

`fields[subscriptions]`

`[string]`

Possible Values: `name, productId, familySharable, state, subscriptionPeriod, reviewNote, groupLevel, subscriptionLocalizations, appStoreReviewScreenshot, group, introductoryOffers, promotionalOffers, offerCodes, prices, pricePoints, promotedPurchase, subscriptionAvailability, winBackOffers, images`

`include`

`[string]`

Possible Values: `subscriptions, subscriptionGroupLocalizations`

`limit[subscriptionGroupLocalizations]`

`integer`

Maximum: `50`

`limit[subscriptions]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

SubscriptionGroupResponse

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

Modify a Subscription Group

Update the reference name for a specific subscription group.

Delete a Subscription Group

Delete a specific empty subscription group.

List All Subscription Group Localizations

Get a list of all localized metadata for a specific subscription group.

List All Subscriptions for a Subscription Group

Get a list of all auto-renewable subscriptions in a subscription group.

