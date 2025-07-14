

- StoreKit
- Transaction
- Transaction.AdvancedCommerceInfo
-  Transaction.AdvancedCommerceInfo.Item 

Structure

# Transaction.AdvancedCommerceInfo.Item

The developer-defined product that was purchased.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Item
```

## Topics

### Structures

struct Details

The item details.

### Instance Properties

let details: Transaction.AdvancedCommerceInfo.Item.Details

The item’s details.

let refunds: [Transaction.AdvancedCommerceInfo.Refund]?

The list of refunds that were issued as part of this transaction.

let revocationDate: Date?

The date access to this item was revoked.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

