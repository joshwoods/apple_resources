

- PassKit (Apple Pay and Wallet)
-  PKDisbursementSummaryItem 

Class

# PKDisbursementSummaryItem

A summary item that represents a disbursement.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
class PKDisbursementSummaryItem
```

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

### Setting the summary items

var summaryItems: [PKPaymentSummaryItem]

An array of payment summary item objects that the framework presents to people.

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

class PKInstantFundsOutFeeSummaryItem

A summary item that represents a fee for an instant funds out transfer.

