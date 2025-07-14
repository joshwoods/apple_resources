

- StoreKit
-  SKProductDiscount Deprecated

Class

# SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKProductDiscount
```

Deprecated

Use Product.SubscriptionOffer

## Mentioned in 

Implementing promotional offers in your app

## Overview

You set up introductory and promotional offers in App Store Connect. SKProductDiscount contains the offer information as retrieved from the App Store.

For more information about setting up offers, see Set an introductory offer for an auto-renewable subscription and Set up promotional offers for auto-renewable subscriptions.

## Topics

### Identifying the Discount

var identifier: String?

A string used to uniquely identify a discount offer for a product.

var type: SKProductDiscount.Type

The type of discount offer.

enum Type

Values representing the types of discount offers an app can present.

### Getting Price and Payment Mode

var price: NSDecimalNumber

The discount price of the product in the local currency.

var priceLocale: Locale

The locale used to format the discount price of the product.

var paymentMode: SKProductDiscount.PaymentMode

The payment mode for this product discount.

enum PaymentMode

Values representing the payment modes for a product discount.

### Getting the Discount Duration

var numberOfPeriods: Int

An integer that indicates the number of periods the product discount is available.

var subscriptionPeriod: SKProductSubscriptionPeriod

An object that defines the period for the product discount.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

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

var discounts: [SKProductDiscount]

An array of subscription offers available for the auto-renewable subscription.

Deprecated

