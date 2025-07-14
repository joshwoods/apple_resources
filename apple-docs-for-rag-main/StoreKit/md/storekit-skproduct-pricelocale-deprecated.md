

- StoreKit
- SKProduct
-  priceLocale Deprecated

Instance Property

# priceLocale

The locale used to format the price of the product.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var priceLocale: Locale { get }
```

Deprecated

Use Product.displayPrice

## Discussion

Use the locale to format the price.

## See Also

### Getting Pricing Information

var price: NSDecimalNumber

The cost of the product in the local currency.

Deprecated

var introductoryPrice: SKProductDiscount?

The object containing introductory price information for the product.

Deprecated

var discounts: [SKProductDiscount]

An array of subscription offers available for the auto-renewable subscription.

Deprecated

class SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

Deprecated

