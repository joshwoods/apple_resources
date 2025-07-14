

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentRequest
-  trialBilling 

Instance Property

# trialBilling

The trial billing cycle for the recurring payment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var trialBilling: PKRecurringPaymentSummaryItem? { get set }
```

## Discussion

The trial billing cycle is optional; use it if the purchase has a trial period.

## See Also

### Setting payment summary items

var regularBilling: PKRecurringPaymentSummaryItem

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

class PKRecurringPaymentSummaryItem

An object that defines a summary item for a payment that occurs repeatedly at a specified interval, such as a subscription.

