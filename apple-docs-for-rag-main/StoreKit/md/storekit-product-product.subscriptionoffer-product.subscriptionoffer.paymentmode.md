

- StoreKit
- Product
- Product.SubscriptionOffer
-  Product.SubscriptionOffer.PaymentMode 

Structure

# Product.SubscriptionOffer.PaymentMode

The payment modes for subscription offers that apply to a transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PaymentMode
```

## Mentioned in 

Testing win-back offers in Xcode

## Overview

A payment mode describes how a subscription offer charges its discounted price — whether it charges one time, charges multiple times, or charges nothing because it’s a free trial.

## Topics

### Getting the payment modes

static let freeTrial: Product.SubscriptionOffer.PaymentMode

A payment mode of a product discount that indicates a free trial offer.

static let payAsYouGo: Product.SubscriptionOffer.PaymentMode

A payment mode of a product discount that applies over a single billing period or multiple billing periods.

static let payUpFront: Product.SubscriptionOffer.PaymentMode

A payment mode of a product discount that applies the discount up front.

### Getting a localized description

var localizedDescription: String

The localized text that describes the payment mode.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting price information

let displayPrice: String

The localized string representation of the discounted price of the subscription offer.

let price: Decimal

The decimal representation of the discounted price of the subscription offer.

let paymentMode: Product.SubscriptionOffer.PaymentMode

The offer’s payment mode.

