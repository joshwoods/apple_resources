

- StoreKit
- Product
- 
  - Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
- Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus
-  Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.agreed 

Case

# Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus.agreed

The auto-renewable subscription is subject to a price increase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case agreed
```

## Mentioned in 

Managing Price Increases for Auto-Renewable Subscriptions

## Discussion

There are two types of price increases for auto-renewable subscriptions: those that require customer consent, and those that don’t require customer consent. For a price increase that requires customer consent, this value indicates that the customer consented to the price increase. For a price increase that doesn’t require customer consent, this value indicates that the App Store informed the customer of the price increase and the subscription is subject to the price increase.

For more information about this value, see Managing Price Increases for Auto-Renewable Subscriptions.

## See Also

### Getting Price Increase Status

case noIncreasePending

There’s no pending price increase for the auto-renewable subscription.

case pending

The customer hasn’t yet responded to an auto-renewable subscription price increase that requires customer consent.

