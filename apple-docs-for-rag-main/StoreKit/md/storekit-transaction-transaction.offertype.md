

- StoreKit
- Transaction
-  Transaction.OfferType 

Structure

# Transaction.OfferType

The types of subscription offers for auto-renewable subscriptions.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct OfferType
```

## Overview

You don’t create offer types in Transaction.OfferType. The static values indicate the offer types that the system reports for a transaction.

## Topics

### Getting offer types

static let introductory: Transaction.OfferType

An introductory offer for an auto-renewable subscription.

static let promotional: Transaction.OfferType

A promotional offer for an auto-renewable subscription.

static let code: Transaction.OfferType

An offer with a subscription offer code for an auto-renewable subscription.

static var winBack: Transaction.OfferType

A win-back offer for an auto-renewable subscription.

### Getting a localized description

var localizedDescription: String

The localized text that describes the offer type.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting offer details

let id: String?

A string that identifies the subscription offer that applies to the transaction.

let type: Transaction.OfferType

The type of subscription offer that applies to the transaction.

let paymentMode: Transaction.Offer.PaymentMode?

The payment mode for a subscription offer on an auto-renewable subscription that applies to the transaction.

struct PaymentMode

The payment modes for subscription offers that apply to a transaction.

