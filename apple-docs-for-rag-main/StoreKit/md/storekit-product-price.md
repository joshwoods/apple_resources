

- StoreKit
- Product
-  price 

Instance Property

# price

The decimal representation of the cost of the product, in local currency.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let price: Decimal
```

## Discussion

Use this property to perform arithmetic calculations with the price of the product. For a localized string representation of the price to display to customers, use the displayPrice property instead.

## See Also

### Displaying a product description and price

let displayName: String

The localized display name of the product, if it exists.

let description: String

The localized description of the product.

let displayPrice: String

The localized string representation of the product price, suitable for display.

var priceFormatStyle: Decimal.FormatStyle.Currency

The format style for the numbers in the price of the product.

var subscriptionPeriodFormatStyle: Date.ComponentsFormatStyle

The format style for the date components related to a subscription’s duration.

var subscriptionPeriodUnitFormatStyle: Product.SubscriptionPeriod.Unit.FormatStyle

The format style for subscription period units, such as week, month, or year.

