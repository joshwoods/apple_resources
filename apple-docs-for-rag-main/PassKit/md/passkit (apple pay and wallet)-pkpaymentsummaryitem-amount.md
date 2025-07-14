

- PassKit (Apple Pay and Wallet)
- PKPaymentSummaryItem
-  amount 

Instance Property

# amount

The summary item’s amount.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var amount: NSDecimalNumber { get set }
```

## Discussion

The amount’s currency is specified at the payment level by setting a value for the currencyCode property on PKPaymentRequest.

## See Also

### Describing summary items

var label: String

A short, localized description of the item.

var type: PKPaymentSummaryItemType

The summary item’s type that indicates whether the amount is final.

enum PKPaymentSummaryItemType

Constants that describe the type of the payment summary item, such as final or pending.

