

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  summaryItems 

Instance Property

# summaryItems

An array of payment summary item objects that the framework presents to people.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 15.0+visionOS 1.0+

``` source
var summaryItems: [PKPaymentSummaryItem] { get set }
```

## Discussion

This array must contain one PKPaymentSummaryItem, which contains the amount the individual receives. This may differ from the total amount withdrawn — for example, if the transfer has an associated fee. The framework displays the amount this PKPaymentSummaryItem item represents on the main Apple Pay sheet.

This array may contain up to one PKInstantFundsOutFeeSummaryItem to represent a fee deducted as part of an instant transfer, if applicable. The framework also presents this fee on the main sheet when you initialize the PKDisbursementRequest with the instantFundsOut capability option.

You can specify other line items (such as fees not associated with an instant transfer) using PKPaymentSummaryItem.

If you specify multiple summary items, the last item must represent the total of all previous items.

## See Also

### Setting the summary items

class PKPaymentSummaryItem

An object that defines a summary item in a payment request, taxes, discounts, shipping, a grand total, and the like.

class PKDisbursementSummaryItem

A summary item that represents a disbursement.

class PKInstantFundsOutFeeSummaryItem

A summary item that represents a fee for an instant funds out transfer.

