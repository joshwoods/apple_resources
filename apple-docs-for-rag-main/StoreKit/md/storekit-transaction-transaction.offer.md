

- StoreKit
- Transaction
-  Transaction.Offer 

Structure

# Transaction.Offer

The subscription offers that apply to a transaction.

iOS 17.2+iPadOS 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
struct Offer
```

## Overview

You set up subscription offers for auto-renewable subscriptions in App Store Connect. If a customer redeems an offer, it appears in the offer property of the transaction. If the offer applies to one or more renewal periods, it also appears in the offer property of Product.SubscriptionInfo.RenewalInfo.

For more information about subscription offers, see Providing subscription offers. For information about configuring the various subscription offers in App Store Connect, see:

- Set up offer codes

- Set up introductory offers for auto-renewable subscriptions

- Set up promotional offers for auto-renewable subscriptions

- Set up win-back offers

## Topics

### Getting offer details

let id: String?

A string that identifies the subscription offer that applies to the transaction.

let type: Transaction.OfferType

The type of subscription offer that applies to the transaction.

struct OfferType

The types of subscription offers for auto-renewable subscriptions.

let paymentMode: Transaction.Offer.PaymentMode?

The payment mode for a subscription offer on an auto-renewable subscription that applies to the transaction.

struct PaymentMode

The payment modes for subscription offers that apply to a transaction.

### Instance Properties

let period: Product.SubscriptionPeriod?

The duration of the offer applied to a transaction.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Getting subscription offers

let offer: Transaction.Offer?

A subscription offer that applies to the transaction at the next renewal period.

let eligibleWinBackOfferIDs: [String]

An array of strings that represent identifiers of win-back offers that the customer is eligible to redeem, sorted with the best offers first.

