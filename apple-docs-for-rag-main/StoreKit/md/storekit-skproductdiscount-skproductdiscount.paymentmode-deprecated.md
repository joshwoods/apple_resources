

- StoreKit
- SKProductDiscount
-  SKProductDiscount.PaymentMode Deprecated

Enumeration

# SKProductDiscount.PaymentMode

Values representing the payment modes for a product discount.

iOS 11.2–18.0DeprecatediPadOS 11.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.13.2–15.0DeprecatedtvOS 11.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
enum PaymentMode
```

Deprecated

Use Product.SubscriptionOffer.PaymentMode

## Mentioned in 

Implementing introductory offers in your app

## Overview

The payment mode indicates if the discount price is charged one time, multiple times, or if the discount is a free trial.

The payment mode may determine the wording you choose to phrase the offer in your app’s UI.

## Topics

### Discount Price Payment Modes

case payAsYouGo

A constant that indicates a product discount that applies over a single billing period or multiple billing periods.

case payUpFront

A constant that indicates that the system applies the product discount up front.

case freeTrial

A constant that indicates that the payment mode is a free trial.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Price and Payment Mode

var price: NSDecimalNumber

The discount price of the product in the local currency.

Deprecated

var priceLocale: Locale

The locale used to format the discount price of the product.

Deprecated

var paymentMode: SKProductDiscount.PaymentMode

The payment mode for this product discount.

Deprecated

