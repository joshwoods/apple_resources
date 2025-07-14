

- StoreKit
- Transaction
- Transaction.AdvancedCommerceInfo
-  Transaction.AdvancedCommerceInfo.Refund 

Structure

# Transaction.AdvancedCommerceInfo.Refund

Information about refunds that were issued as part of this transaction.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Refund
```

## Topics

### Structures

struct Reason

The reason for the refund.

struct RefundType

The type of refund.

### Instance Properties

let amount: Decimal

The amount of the refund.

let date: Date

The date the refund was granted.

let reason: Transaction.AdvancedCommerceInfo.Refund.Reason

The reason for the refund.

let type: Transaction.AdvancedCommerceInfo.Refund.RefundType

The type of the refund.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

