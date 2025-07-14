

- StoreKit
- SKProduct
-  discounts Deprecated

Instance Property

# discounts

An array of subscription offers available for the auto-renewable subscription.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var discounts: [SKProductDiscount] { get }
```

Deprecated

Use Product.subscription.promotionalOffers

## Mentioned in 

Implementing promotional offers in your app

## Discussion

The discounts array contains all of the introductory offers and promotional offers that you set up in App Store Connect for this subscription (productIdentifier). It’s up to the logic in your app to decide which offer to present to the user.

For more information about offers, see Implementing promotional offers in your app, and Implementing introductory offers in your app.

## See Also

### Getting Pricing Information

var price: NSDecimalNumber

The cost of the product in the local currency.

Deprecated

var priceLocale: Locale

The locale used to format the price of the product.

Deprecated

var introductoryPrice: SKProductDiscount?

The object containing introductory price information for the product.

Deprecated

class SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

Deprecated

