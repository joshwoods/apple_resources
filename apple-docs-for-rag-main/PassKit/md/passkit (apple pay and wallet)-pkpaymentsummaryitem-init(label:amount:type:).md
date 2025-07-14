

- PassKit (Apple Pay and Wallet)
- PKPaymentSummaryItem
-  init(label:amount:type:) 

Initializer

# init(label:amount:type:)

Initializes and returns a summary item with the given label, amount, and type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    label: String,
    amount: NSDecimalNumber,
    type: PKPaymentSummaryItemType
)
```

## Parameters 

`label`  

A short, localized description of the summary item.

`amount`  

The amount associated with the summary item.

`type`  

The type of the summary item.

## Return Value

A summary item with the given label, amount, and type.

## Discussion

When creating summary items for estimates or charges whose final value isn’t yet known, use a PKPaymentSummaryItemType.pending type. Use zero for the amount of pending items. The payment sheet doesn’t show the value of pending items.

Note

The payment request’s total must include a final value, even if the payment request includes one or more pending summary items. This total represents the total of all the known costs; don’t include the value of any pending items.

## See Also

### Creating summary items

convenience init(label: String, amount: NSDecimalNumber)

Initializes and returns a summary item with the given label and amount.

