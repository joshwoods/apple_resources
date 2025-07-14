

- StoreKit
- Transaction
-  currencyCode Deprecated

Instance Property

# currencyCode

The three-letter ISO 4217 currency code for the price of the product.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedmacOS 12.0–13.0DeprecatedtvOS 15.0–16.0DeprecatedvisionOS 1.0–1.1DeprecatedwatchOS 8.0–9.0Deprecated

``` source
@backDeployed(before: iOS 16.0, macOS 13.0, tvOS 16.0, watchOS 9.0)
var currencyCode: String? { get }
```

Deprecated

Use currency instead. To get the currency code as a string, use the identifier property of currency.

## Discussion

The currencyCode property contains an ISO 4217 alpha-3 string that represents the currency of the price of the product. Use currencyCode to access the currency of the price on systems earlier than iOS 16, iPadOS 16, macOS 13, tvOS 16, and watchOS 9. Otherwise, use currency.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

Don’t use currencyCode to infer the storefront. Use the storefront value in the transaction instead.

For more information on how you set prices, see Set a price for an in-app purchase.

## See Also

### Deprecated

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

var storefrontCountryCode: String

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

Deprecated

