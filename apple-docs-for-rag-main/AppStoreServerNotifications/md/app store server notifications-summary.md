

- App Store Server Notifications
-  summary 

Object

# summary

The payload data for a subscription-renewal-date extension notification.

App Store Server Notifications 2.7+

``` source
object summary
```

## Properties

`requestIdentifier`

requestIdentifier

The `UUID` that represents a specific request to extend a subscription renewal date. This value matches the value you initially specify in the `requestIdentifier` when you call Extend Subscription Renewal Dates for All Active Subscribers in the App Store Server API.

`environment`

environment

The server environment that the notification applies to, either `sandbox` or `production`.

`appAppleId`

appAppleId

The unique identifier of the app that the notification applies to. This property is available for apps that users download from the App Store. It isn’t present in the sandbox environment.

`bundleId`

bundleId

The bundle identifier of the app.

`productId`

productId

The product identifier of the auto-renewable subscription that the subscription-renewal-date extension applies to.

`storefrontCountryCodes`

storefrontCountryCodes

A list of country codes that limits the App Store’s attempt to apply the subscription-renewal-date extension. If this list isn’t present, the subscription-renewal-date extension applies to all storefronts.

`failedCount`

failedCount

The final count of subscriptions that fail to receive a subscription-renewal-date extension.

`succeededCount`

succeededCount

The final count of subscriptions that successfully receive a subscription-renewal-date extension.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

The `summary` object appears in the responseBodyV2DecodedPayload when the notificationType is `RENEWAL_EXTENSION` and the subtype is `SUMMARY`. This notification occurs when the App Store completes your request to extend the subscription renewal date for eligible subscribers. For more information about this request, see Extend Subscription Renewal Dates for All Active Subscribers in the App Store Server API.

## Topics

### Data types

type requestIdentifier

A string that contains a unique identifier for a subscription-renewal-date extension request.

type environment

The server environment, either sandbox or production.

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type productId

The product identifier of the In-App Purchase.

type storefrontCountryCodes

A list of storefront country codes for limiting the storefronts for a subscription-renewal-date extension.

type storefrontCountryCode

The three-letter code that represents the country or region associated with the App Store storefront.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

## See Also

### Response objects for in-app purchases

object data

The payload data that contains app metadata and the signed renewal and transaction information.

