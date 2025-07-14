

- StoreKit
- Product
-  Product.SubscriptionOffer 

Structure

# Product.SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SubscriptionOffer
```

## Mentioned in 

Merchandising win-back offers in your app

## Overview

You set up subscription offers, such as introductory offers and win-back offers, in App Store Connect.

For more information about subscription offers, see Providing subscription offers. For information about configuring the various types of subscription offers in App Store Connect, see:

- Set up offer codes

- Set up introductory offers for auto-renewable subscriptions

- Set up promotional offers for auto-renewable subscriptions

- Set up win-back offers

## Topics

### Getting the subscription offer identifier

let id: String?

The subscription offer identifier.

### Getting the subscription offer type

let type: Product.SubscriptionOffer.OfferType

The type of subscription offer, which can be introductory, promotional, or win-back.

struct OfferType

The types of offers for auto-renewable subscriptions.

### Getting price information

let displayPrice: String

The localized string representation of the discounted price of the subscription offer.

let price: Decimal

The decimal representation of the discounted price of the subscription offer.

let paymentMode: Product.SubscriptionOffer.PaymentMode

The offer’s payment mode.

struct PaymentMode

The payment modes for subscription offers that apply to a transaction.

### Getting the subscription duration

let period: Product.SubscriptionPeriod

The subscription period for the subscription offer.

let periodCount: Int

The number of periods that the subscription offer renews for.

### Creating a subscription offer signature

struct Signature

A cryptographic signature for a promotional offer.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Subscription offers and offer codes

Supporting win-back offers in your app

Re-engage previous subscribers with a free or discounted offer for an auto-renewable subscription, for a specific duration.

Merchandising win-back offers in your app

Present win-back offers to eligible customers in your app with the win-back offer sheet or by implementing custom merchandising.

Supporting subscription offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within your app.

struct OfferType

The types of offers for auto-renewable subscriptions.

