

- StoreKit
- Transaction
-  Transaction.AdvancedCommerceInfo 

Structure

# Transaction.AdvancedCommerceInfo

Metadata for transactions that use the Advanced Commerce API.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct AdvancedCommerceInfo
```

## Topics

### Structures

struct Item

The developer-defined product that was purchased.

struct Offer

Information about the offer that was redeemed as part of the purchase.

struct Refund

Information about refunds that were issued as part of this transaction.

### Instance Properties

let description: String?

let displayName: String?

let estimatedTax: Decimal

let items: [Transaction.AdvancedCommerceInfo.Item]

The items purchased as part of this transaction.

let period: SubscriptionPeriod?

let requestReferenceID: String

let taxCode: String

let taxExclusivePrice: Decimal

let taxRate: Decimal

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

