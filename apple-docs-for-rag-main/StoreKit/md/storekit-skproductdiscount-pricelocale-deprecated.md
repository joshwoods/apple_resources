

- StoreKit
- SKProductDiscount
-  priceLocale Deprecated

Instance Property

# priceLocale

The locale used to format the discount price of the product.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var priceLocale: Locale { get }
```

Deprecated

Use Product.SubscriptionOffer.displayPrice

## Discussion

Use the locale to format the price.

## See Also

### Getting Price and Payment Mode

var price: NSDecimalNumber

The discount price of the product in the local currency.

Deprecated

var paymentMode: SKProductDiscount.PaymentMode

The payment mode for this product discount.

Deprecated

enum PaymentMode

Values representing the payment modes for a product discount.

Deprecated

