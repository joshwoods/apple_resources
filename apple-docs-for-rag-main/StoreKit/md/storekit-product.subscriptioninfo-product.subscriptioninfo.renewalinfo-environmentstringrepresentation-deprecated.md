

- StoreKit
- Product
- 
  - Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  environmentStringRepresentation Deprecated

Instance Property

# environmentStringRepresentation

The string representation of the server environment that signs the renewal information for an auto-renewable subscription.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 12.0–13.0DeprecatedtvOS 15.0–16.0DeprecatedwatchOS 8.0–9.0Deprecated

``` source
@backDeployed(before: iOS 16.0, macOS 13.0, tvOS 16.0, watchOS 9.0, macCatalyst 16.0)
var environmentStringRepresentation: String { get }
```

Deprecated

Use the environment property instead

## See Also

### Deprecated

var offerID: String?

A string that identifies an offer applied to the next subscription period.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the next subscription period.

Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var offerPaymentModeStringRepresentation: String?Deprecated

var offerPeriodStringRepresentation: String?

The string representation of the subscription offer period applied to the next billing period.

Deprecated

