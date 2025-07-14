

- StoreKit
- Transaction
-  Transaction.Reason 

Structure

# Transaction.Reason

A cause of a purchase transaction, indicating whether it’s a customer’s purchase or an auto-renewable subscription renewal that the system initiates.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Reason
```

## Topics

### Transaction reasons

static let purchase: Transaction.Reason

A transaction reason that indicates a purchase is initiated by a customer.

static let renewal: Transaction.Reason

A transaction reason that indicates the App Store server initiated a purchase transaction to renew an auto-renewable subscription.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting transaction reason

let reason: Transaction.Reason

The cause of the purchase transaction, whether it’s a customer’s purchase or an auto-renewable subscription renewal that the system initiates.

