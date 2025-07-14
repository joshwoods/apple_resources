

- PassKit (Apple Pay and Wallet)
- PKPaymentSummaryItem
-  type 

Instance Property

# type

The summary item’s type that indicates whether the amount is final.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var type: PKPaymentSummaryItemType { get set }
```

## Discussion

This property defaults to a PKPaymentSummaryItemType.final type. See PKPaymentSummaryItemType for other values.

## See Also

### Describing summary items

var label: String

A short, localized description of the item.

var amount: NSDecimalNumber

The summary item’s amount.

enum PKPaymentSummaryItemType

Constants that describe the type of the payment summary item, such as final or pending.

