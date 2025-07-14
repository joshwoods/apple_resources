

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.Status
-  renewalInfo 

Instance Property

# renewalInfo

The signed renewal information for the auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let renewalInfo: VerificationResult
```

## Mentioned in 

Managing Price Increases for Auto-Renewable Subscriptions

Testing In-App Purchases in Xcode

## See Also

### Getting subscription status information

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let transaction: VerificationResult&lt;Transaction>

The latest transaction for the subscription group.

struct RenewalInfo

The renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

