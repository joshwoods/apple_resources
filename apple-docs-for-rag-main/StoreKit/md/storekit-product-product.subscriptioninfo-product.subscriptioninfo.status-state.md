

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.Status
-  state 

Instance Property

# state

The renewal state of the auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let state: Product.SubscriptionInfo.RenewalState
```

## See Also

### Getting the renewal or expiration state

let autoRenewPreference: String?

The product ID of the auto-renewable subscription that will automatically renew.

let willAutoRenew: Bool

A Boolean value that indicates whether the subscription automatically renews in the next period.

let expirationReason: Product.SubscriptionInfo.RenewalInfo.ExpirationReason?

The reason the auto-renewable subscription expired.

struct ExpirationReason

The reasons for auto-renewable subscription expirations.

