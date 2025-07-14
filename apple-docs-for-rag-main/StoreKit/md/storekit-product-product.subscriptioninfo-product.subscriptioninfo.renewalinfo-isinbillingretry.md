

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  isInBillingRetry 

Instance Property

# isInBillingRetry

A Boolean value that indicates whether an auto-renewable subscription is in the billing retry period.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let isInBillingRetry: Bool
```

## Mentioned in 

Testing failing subscription renewals and In-App Purchases

## Discussion

This field indicates whether Apple is attempting to automatically renew an expired subscription. If a subscription expires due to a billing issue, a value of `true` indicates that Apple is still trying to renew the subscription. If the subscription is in a billing grace period, the optional gracePeriodExpirationDate contains a date.

Use the isInBillingRetry value along with expirationReason for more insight, as the following table shows:

| Values | Description |
|----|----|
| isInBillingRetry is `false,`  expirationReason is `nil` | The auto-renewable subscription is active and not in a billing retry period.  The subscription is entitled to service. |
| isInBillingRetry is `true,`  expirationReason is billingError,  gracePeriodExpirationDate has a date | The auto-renewable subscription is in a billing grace period.  The subscription is entitled to service until the date in gracePeriodExpirationDate. |
| isInBillingRetry is `true,`  expirationReason is billingError,  gracePeriodExpirationDate is `nil` | The auto-renewable subscription is in a billing retry period.  The subscription is not entitled to service. |
| isInBillingRetry is `false,`  expirationReason is billingError | The auto-renewable subscription expired and billing retry wasn’t able to recover the subscription.  The subscription is not entitled to service. |

## See Also

### Getting billing status

let gracePeriodExpirationDate: Date?

The date the billing grace period expires for the auto-renewable subscription.

