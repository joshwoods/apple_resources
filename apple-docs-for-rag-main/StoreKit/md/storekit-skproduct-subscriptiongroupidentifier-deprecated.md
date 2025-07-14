

- StoreKit
- SKProduct
-  subscriptionGroupIdentifier Deprecated

Instance Property

# subscriptionGroupIdentifier

The identifier of the subscription group to which the subscription belongs.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedtvOS 12.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var subscriptionGroupIdentifier: String? { get }
```

Deprecated

Use Product.subscription.subscriptionGroupID

## Mentioned in 

Handling Subscriptions Billing

## Discussion

Auto-renewable subscriptions always belong to a subscription group. You create the subscription group identifiers in App Store Connect before you create and add an auto-renewable subscription. For more information about subscription groups, see Offer auto-renewable subscriptions.

This property is `nil` if the SKProduct isn’t an auto-renewable subscription.

## See Also

### Getting Subscription Information

var subscriptionPeriod: SKProductSubscriptionPeriod?

The period details for products that are subscriptions.

Deprecated

class SKProductSubscriptionPeriod

An object containing the subscription period duration information.

Deprecated

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

Deprecated

