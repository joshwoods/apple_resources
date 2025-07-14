

- App Store Connect API
-  List All Subscription Groups for an App 

Web Service Endpoint

# List All Subscription Groups for an App

Get a list of subscription groups for a specific app.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/apps/{id}/subscriptionGroups
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

`filter[referenceName]`

`[string]`

`filter[subscriptions.state]`

`[string]`

Possible Values: `MISSING_METADATA, READY_TO_SUBMIT, WAITING_FOR_REVIEW, IN_REVIEW, DEVELOPER_ACTION_NEEDED, PENDING_BINARY_APPROVAL, APPROVED, DEVELOPER_REMOVED_FROM_SALE, REMOVED_FROM_SALE, REJECTED`

`include`

`[string]`

Possible Values: `subscriptions, subscriptionGroupLocalizations`

`limit`

`integer`

Maximum: `200`

`limit[subscriptionGroupLocalizations]`

`integer`

Maximum: `50`

`limit[subscriptions]`

`integer`

Maximum: `50`

`sort`

`[string]`

Possible Values: `referenceName, -referenceName`

## Response Codes

` 200 ``OK`

SubscriptionGroupsResponse

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

Read Subscription Group Information

Get the details of a specific subscription group.

Modify a Subscription Group

Update the reference name for a specific subscription group.

Delete a Subscription Group

Delete a specific empty subscription group.

List All Subscription Group Localizations

Get a list of all localized metadata for a specific subscription group.

List All Subscriptions for a Subscription Group

Get a list of all auto-renewable subscriptions in a subscription group.

