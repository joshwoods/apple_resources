

- StoreKit
- Transaction
- Transaction.AdvancedCommerceInfo
-  Transaction.AdvancedCommerceInfo.Offer 

Structure

# Transaction.AdvancedCommerceInfo.Offer

Information about the offer that was redeemed as part of the purchase.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Offer
```

## Topics

### Structures

struct Reason

The reasons why subscription offers are applied to the purchase of auto-renewable subscriptions.

### Instance Properties

let period: SubscriptionPeriod

The duration of the offer.

let periodCount: Int

The number of periods the system applies the offer.

let price: Decimal

The discounted price under the offer.

let reason: Transaction.AdvancedCommerceInfo.Offer.Reason

The reason the offer was applied.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

