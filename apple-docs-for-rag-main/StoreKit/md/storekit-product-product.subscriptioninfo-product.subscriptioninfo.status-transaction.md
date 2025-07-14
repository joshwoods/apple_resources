

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.Status
-  transaction 

Instance Property

# transaction

The latest transaction for the subscription group.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let transaction: VerificationResult
```

## See Also

### Getting subscription status information

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let renewalInfo: VerificationResult&lt;Product.SubscriptionInfo.RenewalInfo>

The signed renewal information for the auto-renewable subscription.

struct RenewalInfo

The renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

