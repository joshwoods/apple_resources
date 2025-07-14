

- StoreKit
- Transaction
-  storefrontCountryCode Deprecated

Instance Property

# storefrontCountryCode

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

iOS 15.0–17.0DeprecatediPadOS 15.0–17.0DeprecatedMac Catalyst 15.0–17.0DeprecatedmacOS 12.0–14.0DeprecatedtvOS 15.0–17.0DeprecatedwatchOS 8.0–10.0Deprecated

``` source
@backDeployed(before: iOS 17.0, macOS 14.0, tvOS 17.0, watchOS 10.0, macCatalyst 17.0)
var storefrontCountryCode: String { get }
```

Deprecated

Use storefront instead.

## Discussion

This property uses the ISO 3166-1 alpha-3 country code representation.

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

var offerPaymentModeStringRepresentation: String?

The string representation of the payment mode for a subscription offer.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the current subscription period.

Deprecated

var reasonStringRepresentation: String

The string representation of the transaction reason.

Deprecated

