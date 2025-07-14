

- App Store Server Notifications
-  storefrontCountryCodes 

Type

# storefrontCountryCodes

A list of storefront country codes for limiting the storefronts for a subscription-renewal-date extension.

App Store Server Notifications 2.7+

``` source
[storefrontCountryCode] storefrontCountryCodes
```

## Attributes 

Maximum length: `3`

## Discussion

If you provide a list of storefronts when you call the Extend Subscription Renewal Dates for All Active Subscribers endpoint, the notification returns only those storefronts. If you don’t use the `storefrontCountryCodes`, the subscription-renewal-date extension applies to all storefronts.

For information about providing the list of storefronts, see MassExtendRenewalDateRequest.

## See Also

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

type storefrontCountryCode

The three-letter code that represents the country or region associated with the App Store storefront.

type failedCount

The count of subscriptions that fail to receive a subscription-renewal-date extension.

type succeededCount

The count of subscriptions that successfully receive a subscription-renewal-date extension.

