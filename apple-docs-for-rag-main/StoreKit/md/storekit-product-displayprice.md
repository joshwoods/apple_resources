

- StoreKit
- Product
-  displayPrice 

Instance Property

# displayPrice

The localized string representation of the product price, suitable for display.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let displayPrice: String
```

## Discussion

Use this string to display the price, formatted for the locale. The storefront that the user’s device is connected to determines the locale. For more information, see Storefront.

To perform arithmetic calculations with the price, use the price property instead.

## See Also

### Displaying a product description and price

let displayName: String

The localized display name of the product, if it exists.

let description: String

The localized description of the product.

let price: Decimal

The decimal representation of the cost of the product, in local currency.

var priceFormatStyle: Decimal.FormatStyle.Currency

The format style for the numbers in the price of the product.

var subscriptionPeriodFormatStyle: Date.ComponentsFormatStyle

The format style for the date components related to a subscription’s duration.

var subscriptionPeriodUnitFormatStyle: Product.SubscriptionPeriod.Unit.FormatStyle

The format style for subscription period units, such as week, month, or year.

