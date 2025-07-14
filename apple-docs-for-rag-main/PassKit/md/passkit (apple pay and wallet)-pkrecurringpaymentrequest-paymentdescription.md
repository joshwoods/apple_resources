

- PassKit (Apple Pay and Wallet)
- PKRecurringPaymentRequest
-  paymentDescription 

Instance Property

# paymentDescription

A description that you provide of the recurring payment and that Apple Pay displays to the user in the payment sheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var paymentDescription: String { get set }
```

## Discussion

Provide a display name for the recurring payment, for example, “Apple News+”.

## See Also

### Describing a recurring payment

var billingAgreement: String?

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

