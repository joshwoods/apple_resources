

- StoreKit
- Product
-  displayName 

Instance Property

# displayName

The localized display name of the product, if it exists.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let displayName: String
```

## Discussion

The storefront of the device determines the language of the display name, not the preferred language set on the device. For more information, see Storefront.

Note

When you create a new product in App Store Connect or in a StoreKit configuration file, you can test it before you add a product localization. The displayName value is an empty string until you add a localization. For more information on localizations, see Add and remove localizations.

## See Also

### Displaying a product description and price

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

var subscriptionPeriodUnitFormatStyle: Product.SubscriptionPeriod.Unit.FormatStyle

The format style for subscription period units, such as week, month, or year.

