

- StoreKit
- Product
- Product.SubscriptionOffer
-  periodCount 

Instance Property

# periodCount

The number of periods that the subscription offer renews for.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let periodCount: Int
```

## Discussion

If the payment mode is payAsYouGo, the period count represents the number of periods the subscription renews at the discounted price.

The period count is 1 for offers with payment modes freeTrial and payUpFront.

## See Also

### Getting the subscription duration

let period: Product.SubscriptionPeriod

The subscription period for the subscription offer.

