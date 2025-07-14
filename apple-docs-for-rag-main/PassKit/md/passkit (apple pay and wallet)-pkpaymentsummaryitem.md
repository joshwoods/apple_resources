

- PassKit (Apple Pay and Wallet)
-  PKPaymentSummaryItem 

Class

# PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPaymentSummaryItem
```

## Overview

For shipping cost, use the PKShippingMethod subclass.

## Topics

### Creating summary items

convenience init(label: String, amount: NSDecimalNumber)

Initializes and returns a summary item with the given label and amount.

convenience init(label: String, amount: NSDecimalNumber, type: PKPaymentSummaryItemType)

Initializes and returns a summary item with the given label, amount, and type.

### Describing summary items

var label: String

A short, localized description of the item.

var amount: NSDecimalNumber

The summary item’s amount.

var type: PKPaymentSummaryItemType

The summary item’s type that indicates whether the amount is final.

enum PKPaymentSummaryItemType

Constants that describe the type of the payment summary item, such as final or pending.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PKAutomaticReloadPaymentSummaryItem
- PKDeferredPaymentSummaryItem
- PKDisbursementSummaryItem
- PKInstantFundsOutFeeSummaryItem
- PKRecurringPaymentSummaryItem
- PKShippingMethod

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

class PKDisbursementSummaryItem

A summary item that represents a disbursement.

class PKInstantFundsOutFeeSummaryItem

A summary item that represents a fee for an instant funds out transfer.

