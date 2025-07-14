

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalState
-  inGracePeriod 

Type Property

# inGracePeriod

The subscription is in a billing grace period state.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let inGracePeriod: Product.SubscriptionInfo.RenewalState
```

## Discussion

An auto-renewable subscription in this state is entitled to service.

## See Also

### Getting the renewal state

static let subscribed: Product.SubscriptionInfo.RenewalState

The customer is currently subscribed.

static let expired: Product.SubscriptionInfo.RenewalState

The subscription expired.

static let inBillingRetryPeriod: Product.SubscriptionInfo.RenewalState

The subscription is in a billing retry period.

static let revoked: Product.SubscriptionInfo.RenewalState

The App Store has revoked the customer’s access to the subscription group.

