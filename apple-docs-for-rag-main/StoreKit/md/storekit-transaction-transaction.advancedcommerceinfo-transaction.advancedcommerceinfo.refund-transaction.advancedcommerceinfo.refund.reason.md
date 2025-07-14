

- StoreKit
- Transaction
- Transaction.AdvancedCommerceInfo
- Transaction.AdvancedCommerceInfo.Refund
-  Transaction.AdvancedCommerceInfo.Refund.Reason 

Structure

# Transaction.AdvancedCommerceInfo.Refund.Reason

The reason for the refund.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Reason
```

## Topics

### Type Properties

static let legal: Transaction.AdvancedCommerceInfo.Refund.Reason

The customer requested a refund based on a legal reason.

static let modifyItems: Transaction.AdvancedCommerceInfo.Refund.Reason

static let other: Transaction.AdvancedCommerceInfo.Refund.Reason

The customer requested a refund for other reasons.

static let unfulfilled: Transaction.AdvancedCommerceInfo.Refund.Reason

The customer had issues with receiving or using the in-app purchase.

static let unintended: Transaction.AdvancedCommerceInfo.Refund.Reason

The customer didn’t intend to make the in-app purchase.

static let unsatisfied: Transaction.AdvancedCommerceInfo.Refund.Reason

The customer wasn’t satisfied with the in-app purchase.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

