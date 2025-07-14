

- StoreKit
- SKProduct
-  price Deprecated

Instance Property

# price

The cost of the product in the local currency.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var price: NSDecimalNumber { get }
```

Deprecated

Use Product.displayPrice

## Discussion

Your app can format the price using a number formatter, as shown in the following sample code:

- Swift
- Objective-C

```
let numberFormatter = NumberFormatter()
numberFormatter.numberStyle = .currency
numberFormatter.locale = product.priceLocale
let formattedString = numberFormatter.string(from: product.price)
```

```
NSNumberFormatter *numberFormatter = [[NSNumberFormatter alloc] init];
[numberFormatter setFormatterBehavior:NSNumberFormatterBehavior10_4];
[numberFormatter setNumberStyle:NSNumberFormatterCurrencyStyle];
[numberFormatter setLocale:product.priceLocale];
NSString *formattedString = [numberFormatter stringFromNumber:product.price];
```

## See Also

### Getting Pricing Information

var priceLocale: Locale

The locale used to format the price of the product.

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

