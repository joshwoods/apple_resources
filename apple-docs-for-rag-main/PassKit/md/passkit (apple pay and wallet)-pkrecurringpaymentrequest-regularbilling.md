

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentRequest
-  regularBilling 

Instance Property

# regularBilling

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var regularBilling: PKRecurringPaymentSummaryItem { get set }
```

## See Also

### Setting payment summary items

var trialBilling: PKRecurringPaymentSummaryItem?

The trial billing cycle for the recurring payment.

class PKRecurringPaymentSummaryItem

An object that defines a summary item for a payment that occurs repeatedly at a specified interval, such as a subscription.

