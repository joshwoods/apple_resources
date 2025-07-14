

- PassKit (Apple Pay and Wallet)
- PKPaymentSummaryItem
-  label 

Instance Property

# label

A short, localized description of the item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var label: String { get set }
```

## Discussion

Provide the label in title case—for example, VAT Tax, Gift Wrap and Card, or Discount.

Omit any punctuation and whitespace after the label. The label is formatted for display by the framework.

## See Also

### Describing summary items

var amount: NSDecimalNumber

The summary item’s amount.

var type: PKPaymentSummaryItemType

The summary item’s type that indicates whether the amount is final.

enum PKPaymentSummaryItemType

Constants that describe the type of the payment summary item, such as final or pending.

