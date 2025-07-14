

- StoreKit
- Transaction
-  offerType Deprecated

Instance Property

# offerType

The subscription offer type for the current subscription period.

iOS 15.0–17.2DeprecatediPadOS 15.0–17.2DeprecatedmacOS 12.0–14.2DeprecatedtvOS 15.0–17.2DeprecatedvisionOS 1.0–1.1DeprecatedwatchOS 8.0–10.2Deprecated

``` source
var offerType: Transaction.OfferType? { get }
```

Deprecated

Use offer instead.

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

If this value is `nil`, there’s no offer applied.

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

var reasonStringRepresentation: String

The string representation of the transaction reason.

Deprecated

var storefrontCountryCode: String

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

Deprecated

