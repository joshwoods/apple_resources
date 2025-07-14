

- PassKit (Apple Pay and Wallet)
- PKPaymentRequestUpdate
-  recurringPaymentRequest 

Instance Property

# recurringPaymentRequest

The recurring payment request to update the payment request with.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var recurringPaymentRequest: PKRecurringPaymentRequest? { get set }
```

## Discussion

The default value is `nil`, which indicates the recurring payment request doesn’t require an update.

Warning

Changing the billingAgreement along with this property causes the framework to invalidate the current payment request, close the payment sheet, and return an error in the completion handler.

You can’t use this property simultaneously with multitoken contexts or automatic reload payment requests.

