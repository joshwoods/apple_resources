

- PassKit (Apple Pay and Wallet)
-  PKDeferredPaymentSummaryItem 

Class

# PKDeferredPaymentSummaryItem

An object that defines a summary item for a payment that occurs at a later date, such as a pre-order.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class PKDeferredPaymentSummaryItem
```

## Topics

### Setting the payment date

var deferredDate: Date

The date, in the future, of the payment.

## Relationships

### Inherits From

- PKPaymentSummaryItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Setting payment summary items

var deferredBilling: PKDeferredPaymentSummaryItem

An object that contains details about the deferred payment.

