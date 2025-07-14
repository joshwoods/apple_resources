

- StoreKit
- SKProduct
-  introductoryPrice Deprecated

Instance Property

# introductoryPrice

The object containing introductory price information for the product.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var introductoryPrice: SKProductDiscount? { get }
```

Deprecated

Use Product.subscription.introductionaryOffer

## Mentioned in 

Implementing introductory offers in your app

## Discussion

If you’ve set up introductory prices in App Store Connect, the introductory price property will be populated. This property is `nil` if the product has no introductory price.

Before displaying UI that offers the introductory price, you must first determine if the user is eligible to receive it. See Implementing introductory offers in your app for information on determining eligibility and displaying introductory prices.

## See Also

### Getting Pricing Information

var price: NSDecimalNumber

The cost of the product in the local currency.

Deprecated

var priceLocale: Locale

The locale used to format the price of the product.

Deprecated

var discounts: [SKProductDiscount]

An array of subscription offers available for the auto-renewable subscription.

Deprecated

class SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

Deprecated

