

- StoreKit
- Product
- Product.PurchaseOption
- Product.PurchaseOption.SubscriptionRenewalBehavior
-  Product.PurchaseOption.SubscriptionRenewalBehavior.cancelImmediately 

Case

# Product.PurchaseOption.SubscriptionRenewalBehavior.cancelImmediately

A subscription-renewal behavior in the testing environment that cancels the subscription, resulting in only one subscription period.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case cancelImmediately
```

## Discussion

Choose this option for test cases that require an auto-renewable subscription that won’t renew.

## See Also

### Renewal behaviors in the testing environment

case renewUntilNow

A subscription-renewal behavior in the testing environment that allows the subscription to renew continuously, up to the current date.

