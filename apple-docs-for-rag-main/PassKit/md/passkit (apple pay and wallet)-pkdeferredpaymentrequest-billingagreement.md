

- PassKit (Apple Pay and Wallet)
- PKDeferredPaymentRequest
-  billingAgreement 

Instance Property

# billingAgreement

The localized billing agreement the framework displays to the user prior to payment authorization.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var billingAgreement: String? { get set }
```

## Discussion

This may include additional details about the cancellation period or penalties for late cancellation. This value is optional.

## See Also

### Describing a deferred payment

var freeCancellationDate: Date?

The date before which you must cancel a deferred payment without incurring any cancellation charges.

var paymentDescription: String

A description of the deferred payment.

var freeCancellationDateTimeZone: TimeZone?

The time zone at the destination location of the payment.

