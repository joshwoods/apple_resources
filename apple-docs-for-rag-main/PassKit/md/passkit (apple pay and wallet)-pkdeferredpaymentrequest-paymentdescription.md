

- PassKit (Apple Pay and Wallet)
- PKDeferredPaymentRequest
-  paymentDescription 

Instance Property

# paymentDescription

A description of the deferred payment.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var paymentDescription: String { get set }
```

## Discussion

Use a plain language description that explains what the payment is for, for example “Hotel stay, 2 nights.”

## See Also

### Describing a deferred payment

var freeCancellationDate: Date?

The date before which you must cancel a deferred payment without incurring any cancellation charges.

var billingAgreement: String?

The localized billing agreement the framework displays to the user prior to payment authorization.

var freeCancellationDateTimeZone: TimeZone?

The time zone at the destination location of the payment.

