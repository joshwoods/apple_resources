

- StoreKit
- Product
- 
  - Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
- Product.SubscriptionInfo.RenewalInfo.ExpirationReason
-  productUnavailable 

Type Property

# productUnavailable

The auto-renewable subscription expired because the product was unavailable for purchase at the time of the renewal.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let productUnavailable: Product.SubscriptionInfo.RenewalInfo.ExpirationReason
```

## See Also

### Getting the expiration reason

static let autoRenewDisabled: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired because the customer voluntarily canceled their subscription.

static let billingError: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired because of a billing error.

static let didNotConsentToPriceIncrease: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The subscription expired because the customer didn’t consent to an auto-renewable subscription price increase that requires customer consent.

static let unknown: Product.SubscriptionInfo.RenewalInfo.ExpirationReason

The auto-renewable subscription expired for an unknown reason.

