

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentSummaryItem
-  startDate 

Instance Property

# startDate

The date of the first payment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
var startDate: Date? { get set }
```

## Discussion

The default value is `nil` which requests the first payment as part of the initial transaction.

## See Also

### Setting the payment period

var endDate: Date?

The date of the final payment.

