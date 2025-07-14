

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  expirationReason 

Instance Property

# expirationReason

The reason the auto-renewable subscription expired.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let expirationReason: Product.SubscriptionInfo.RenewalInfo.ExpirationReason?
```

## Mentioned in 

Managing Price Increases for Auto-Renewable Subscriptions

## Discussion

This optional value is `nil` if the auto-renewable subscription is active and hasn’t expired.

## See Also

### Getting the renewal or expiration state

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let autoRenewPreference: String?

The product ID of the auto-renewable subscription that will automatically renew.

let willAutoRenew: Bool

A Boolean value that indicates whether the subscription automatically renews in the next period.

struct ExpirationReason

The reasons for auto-renewable subscription expirations.

