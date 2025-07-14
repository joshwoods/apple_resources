

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  willAutoRenew 

Instance Property

# willAutoRenew

A Boolean value that indicates whether the subscription automatically renews in the next period.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let willAutoRenew: Bool
```

## Mentioned in 

Supporting win-back offers in your app

## See Also

### Getting the renewal or expiration state

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let autoRenewPreference: String?

The product ID of the auto-renewable subscription that will automatically renew.

let expirationReason: Product.SubscriptionInfo.RenewalInfo.ExpirationReason?

The reason the auto-renewable subscription expired.

struct ExpirationReason

The reasons for auto-renewable subscription expirations.

