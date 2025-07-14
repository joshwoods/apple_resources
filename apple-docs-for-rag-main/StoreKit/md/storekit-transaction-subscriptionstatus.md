

- StoreKit
- Transaction
-  subscriptionStatus 

Instance Property

# subscriptionStatus

An array that contains status information for a subscription group, including renewal and transaction information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 17.0, macOS 14.0, tvOS 17.0, watchOS 10.0)
var subscriptionStatus: Product.SubscriptionInfo.Status? { get async }
```

## Discussion

This value is `nil` if the product in the transaction isn’t an auto-renewable subscription, specifically, if the productType is anything other than autoRenewable.

The array can have more than one subscription status, for example, if your subscription supports Family Sharing. Provide the customer with service for the subscription based on the highest level of service where the subscription status is subscribed.

