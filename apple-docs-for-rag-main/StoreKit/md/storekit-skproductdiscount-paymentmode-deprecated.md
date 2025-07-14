

- StoreKit
- SKProductDiscount
-  paymentMode Deprecated

Instance Property

# paymentMode

The payment mode for this product discount.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var paymentMode: SKProductDiscount.PaymentMode { get }
```

Deprecated

Use Product.SubscriptionOffer.paymentMode

## Discussion

The payment mode indicates how the product discount price is charged:

- One or more times, for SKProductDiscount.PaymentMode.payAsYouGo mode

- Once in advance, for SKProductDiscount.PaymentMode.payUpFront mode

- No initial charge, for SKProductDiscount.PaymentMode.freeTrial mode.

Use the payment mode to display an accurate description of the product discount in your UI. For design guidance, see Human Interface Guidelines > In-App Purchase.

## See Also

### Getting Price and Payment Mode

var price: NSDecimalNumber

The discount price of the product in the local currency.

Deprecated

var priceLocale: Locale

The locale used to format the discount price of the product.

Deprecated

enum PaymentMode

Values representing the payment modes for a product discount.

Deprecated

