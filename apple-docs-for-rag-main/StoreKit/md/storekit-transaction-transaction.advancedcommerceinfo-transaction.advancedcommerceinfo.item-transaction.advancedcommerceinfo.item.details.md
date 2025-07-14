

- StoreKit
- Transaction
- Transaction.AdvancedCommerceInfo
- Transaction.AdvancedCommerceInfo.Item
-  Transaction.AdvancedCommerceInfo.Item.Details 

Structure

# Transaction.AdvancedCommerceInfo.Item.Details

The item details.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Details
```

## Topics

### Instance Properties

let description: String

The description of the item.

let displayName: String

The display name of the item.

let offer: Transaction.AdvancedCommerceInfo.Offer?

The offer applied to the purchase of this item, if any.

let price: Decimal

The price of the item.

let sku: String

Unique identifier for the item.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

