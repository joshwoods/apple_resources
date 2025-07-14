

- StoreKit
- Transaction
-  offerPaymentModeStringRepresentation Deprecated

Instance Property

# offerPaymentModeStringRepresentation

The string representation of the payment mode for a subscription offer.

iOS 15.0–17.2DeprecatediPadOS 15.0–17.2DeprecatedmacOS 12.0–14.2DeprecatedtvOS 15.0–17.2DeprecatedvisionOS 1.0–1.1DeprecatedwatchOS 8.0–10.2Deprecated

``` source
@backDeployed(before: iOS 17.2, macOS 14.2, tvOS 17.2, watchOS 10.2)
var offerPaymentModeStringRepresentation: String? { get }
```

Deprecated

Use `paymentMode` instead.

## See Also

### Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var environmentStringRepresentation: String

A string representation of the server environment.

Deprecated

var offerID: String?

A string that identifies an offer applied to the current subscription.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the current subscription period.

Deprecated

var reasonStringRepresentation: String

The string representation of the transaction reason.

Deprecated

var storefrontCountryCode: String

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

Deprecated

