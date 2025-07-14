

- StoreKit
- Product
-  subscriptionPeriodFormatStyle 

Instance Property

# subscriptionPeriodFormatStyle

The format style for the date components related to a subscription’s duration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 16.0, macOS 13.0, tvOS 16.0, watchOS 9.0, macCatalyst 16.0)
var subscriptionPeriodFormatStyle: Date.ComponentsFormatStyle { get }
```

## Discussion

Use this format style to format text that describes a subscription period, including its length and unit, such as “1 week”, “2 months”, and so on. Use this style with the formatted(_:referenceDate:) method on Product.SubscriptionPeriod to format the subscription period for the App Store locale.

Note

When using subscriptionPeriodFormatStyle on systems earlier than iOS 16, macOS 13, tvOS 16, and watchOS 9, the property may return a format style with a sentinel locale identifier of `“xx_XX”` in uncommon cases, including if the server has an error, or while testing your app using StoreKit Testing in Xcode. For StoreKit testing, use a later OS version.

## See Also

### Displaying a product description and price

let displayName: String

The localized display name of the product, if it exists.

let description: String

The localized description of the product.

let displayPrice: String

The localized string representation of the product price, suitable for display.

let price: Decimal

The decimal representation of the cost of the product, in local currency.

var priceFormatStyle: Decimal.FormatStyle.Currency

The format style for the numbers in the price of the product.

var subscriptionPeriodUnitFormatStyle: Product.SubscriptionPeriod.Unit.FormatStyle

The format style for subscription period units, such as week, month, or year.

