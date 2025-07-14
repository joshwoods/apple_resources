

- StoreKit
- Transaction
-  offerID Deprecated

Instance Property

# offerID

A string that identifies an offer applied to the current subscription.

iOS 15.0–17.2DeprecatediPadOS 15.0–17.2DeprecatedmacOS 12.0–14.2DeprecatedtvOS 15.0–17.2DeprecatedvisionOS 1.0–1.1DeprecatedwatchOS 8.0–10.2Deprecated

``` source
var offerID: String? { get }
```

Deprecated

Use offer instead.

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

This value is `nil` if there isn’t an offer, or if the offer type is introductory.

If the offer type is promotional, this value contains the promotional offer identifier you set up in App Store Connect. For more information about promotional offers, see Set up promotional offers for auto-renewable subscriptions.

If the offer type is code, this value contains the reference name of the offer code you set up in App Store Connect. For more information about offer codes, see Set up offer codes.

## See Also

### Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var environmentStringRepresentation: String

A string representation of the server environment.

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

