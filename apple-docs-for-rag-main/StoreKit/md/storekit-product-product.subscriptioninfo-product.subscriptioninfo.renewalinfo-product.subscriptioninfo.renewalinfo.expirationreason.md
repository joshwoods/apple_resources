

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  Product.SubscriptionInfo.RenewalInfo.ExpirationReason 

Structure

# Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The reasons for auto-renewable subscription expirations.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ExpirationReason
```

## Topics

### Getting the expiration reason

static let autoRenewDisabled: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired because the customer voluntarily canceled their subscription.

static let billingError: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired because of a billing error.

static let didNotConsentToPriceIncrease: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The subscription expired because the customer didn’t consent to an auto-renewable subscription price increase that requires customer consent.

static let productUnavailable: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired because the product was unavailable for purchase at the time of the renewal.

static let unknown: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired for an unknown reason.

### Getting a localized description

var localizedDescription: String

The localized text that describes the expiration reason.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the renewal or expiration state

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let autoRenewPreference: String?

The product ID of the auto-renewable subscription that will automatically renew.

let willAutoRenew: Bool

A Boolean value that indicates whether the subscription automatically renews in the next period.

let expirationReason: Product.SubscriptionInfo.RenewalInfo.ExpirationReason?

The reason the auto-renewable subscription expired.

