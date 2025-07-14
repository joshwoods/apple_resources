

- StoreKit
- SKProductDiscount
-  price Deprecated

Instance Property

# price

The discount price of the product in the local currency.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var price: NSDecimalNumber { get }
```

Deprecated

Use Product.SubscriptionOffer.displayPrice

## Discussion

Use the priceLocale to format the price.

## See Also

### Getting Price and Payment Mode

var priceLocale: Locale

The locale used to format the discount price of the product.

Deprecated

var paymentMode: SKProductDiscount.PaymentMode

The payment mode for this product discount.

Deprecated

enum PaymentMode

Values representing the payment modes for a product discount.

Deprecated

