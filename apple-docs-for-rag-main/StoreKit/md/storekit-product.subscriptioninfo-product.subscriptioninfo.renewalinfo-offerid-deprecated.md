

- StoreKit
- Product
- 
  - Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  offerID Deprecated

Instance Property

# offerID

A string that identifies an offer applied to the next subscription period.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
var offerID: String? { get }
```

Deprecated

Use the offer property instead

## Mentioned in 

Supporting subscription offer codes in your app

## Discussion

This value is `nil` if there isn’t an offer, or if the offer type is introductory.

If the offer type is promotional, this value contains the promotional offer identifier you set up in App Store Connect. For more information about promotional offers, see Set up promotional offers for auto-renewable subscriptions.

If the offer type is code, this value contains the reference name of the offer code you set up in App Store Connect. For more information about offer codes, see Set up offer codes.

## See Also

### Deprecated

var environmentStringRepresentation: String

The string representation of the server environment that signs the renewal information for an auto-renewable subscription.

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

