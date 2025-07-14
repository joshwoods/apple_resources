

- StoreKit
- Product
-  subscriptionPeriodUnitFormatStyle 

Instance Property

# subscriptionPeriodUnitFormatStyle

The format style for subscription period units, such as week, month, or year.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var subscriptionPeriodUnitFormatStyle: Product.SubscriptionPeriod.Unit.FormatStyle { get }
```

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

var subscriptionPeriodFormatStyle: Date.ComponentsFormatStyle

The format style for the date components related to a subscription’s duration.

