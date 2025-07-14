

- StoreKit
- Product
- 
  - Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  offerPaymentModeStringRepresentation Deprecated

Instance Property

# offerPaymentModeStringRepresentation

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
@backDeployed(before: iOS 18.0, macOS 15.0, tvOS 18.0, watchOS 11.0, visionOS 2.0)
var offerPaymentModeStringRepresentation: String? { get }
```

Deprecated

Use the offer property instead

## See Also

### Deprecated

var environmentStringRepresentation: String

The string representation of the server environment that signs the renewal information for an auto-renewable subscription.

Deprecated

var offerID: String?

A string that identifies an offer applied to the next subscription period.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the next subscription period.

Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var offerPeriodStringRepresentation: String?

The string representation of the subscription offer period applied to the next billing period.

Deprecated

