

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  gracePeriodExpirationDate 

Instance Property

# gracePeriodExpirationDate

The date the billing grace period expires for the auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let gracePeriodExpirationDate: Date?
```

## Mentioned in 

Testing failing subscription renewals and In-App Purchases

## Discussion

This value is `nil` if the subscription is not in a billing grace period.

This date is present if you enable Billing Grace Period for your app and the subscription is in the billing grace period. Ensure that your app provides full service for the subscription throughout the grace period, which ends on the gracePeriodExpirationDate.

A billing grace period occurs at the start of a billing retry state. Throughout the billing grace period, the value of isInBillingRetry is `true`, which indicates that Apple is attempting to automatically renew the subscription.

For information about supporting Billing Grace Period, see Enable Billing Grace Period for auto-renewable subscriptions and Reducing Involuntary Subscriber Churn.

## See Also

### Getting billing status

let isInBillingRetry: Bool

A Boolean value that indicates whether an auto-renewable subscription is in the billing retry period.

