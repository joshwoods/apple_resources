

- PassKit (Apple Pay and Wallet)
- PKPaymentSummaryItem
-  init(label:amount:) 

Initializer

# init(label:amount:)

Initializes and returns a summary item with the given label and amount.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    label: String,
    amount: NSDecimalNumber
)
```

## Parameters 

`label`  

A short, localized description of the summary item.

`amount`  

The amount associated with the summary item.

## Return Value

A summary item with the given label and amount. The resulting item has a PKPaymentSummaryItemType.final type.

## See Also

### Creating summary items

convenience init(label: String, amount: NSDecimalNumber, type: PKPaymentSummaryItemType)

Initializes and returns a summary item with the given label, amount, and type.

