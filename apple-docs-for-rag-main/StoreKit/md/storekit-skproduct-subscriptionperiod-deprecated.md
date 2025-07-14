

- StoreKit
- SKProduct
-  subscriptionPeriod Deprecated

Instance Property

# subscriptionPeriod

The period details for products that are subscriptions.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var subscriptionPeriod: SKProductSubscriptionPeriod? { get }
```

Deprecated

Use Product.subscription.subscriptionPeriod

## Discussion

This read-only property is `nil` if the product is not a subscription.

A subscription period is described in terms of a unit and the number of units that make up a single period.

## See Also

### Getting Subscription Information

var subscriptionGroupIdentifier: String?

The identifier of the subscription group to which the subscription belongs.

Deprecated

class SKProductSubscriptionPeriod

An object containing the subscription period duration information.

Deprecated

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

Deprecated

