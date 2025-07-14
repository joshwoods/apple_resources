

- App Store Server Notifications
-  requestIdentifier 

Type

# requestIdentifier

A string that contains a unique identifier for a subscription-renewal-date extension request.

App Store Server Notifications 2.7+

``` source
uuid requestIdentifier
```

## Discussion

You originally specify the `requestIdentifier` when you call Extend Subscription Renewal Dates for All Active Subscribers in the App Store Server API.

## See Also

### Data types

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

