

- PassKit (Apple Pay and Wallet)
-  PKPaymentSummaryItemType 

Enumeration

# PKPaymentSummaryItemType

Constants that describe the type of the payment summary item, such as final or pending.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPaymentSummaryItemType
```

## Topics

### Payment summary item types

case final

A summary item that represents a known, final cost.

case pending

A summary item that represents an estimated or unknown cost.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing summary items

var label: String

A short, localized description of the item.

var amount: NSDecimalNumber

The summary item’s amount.

var type: PKPaymentSummaryItemType

The summary item’s type that indicates whether the amount is final.

