

- PassKit (Apple Pay and Wallet)
- PKAutomaticReloadPaymentSummaryItem
-  thresholdAmount 

Instance Property

# thresholdAmount

The balance an account reaches before you apply the automatic reload amount.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var thresholdAmount: NSDecimalNumber { get set }
```

## Discussion

You automatically apply the reload amount to the account when the account balance drops below the threshold amount.

Use the amount property to specify the reload amount.

