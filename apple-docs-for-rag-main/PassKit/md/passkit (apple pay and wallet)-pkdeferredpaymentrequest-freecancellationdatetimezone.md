

- PassKit (Apple Pay and Wallet)
- PKDeferredPaymentRequest
-  freeCancellationDateTimeZone 

Instance Property

# freeCancellationDateTimeZone

The time zone at the destination location of the payment.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
var freeCancellationDateTimeZone: TimeZone? { get set }
```

## Discussion

For a hotel booking, for example, this refers to the local time zone of the hotel. On the payment sheet, this is the time zone the framework uses to format the cancellation date. If you set the `freeCancellationDateTimeZone` date, you need to set freeCancellationDate as well.

## See Also

### Describing a deferred payment

var freeCancellationDate: Date?

The date before which you must cancel a deferred payment without incurring any cancellation charges.

var billingAgreement: String?

The localized billing agreement the framework displays to the user prior to payment authorization.

var paymentDescription: String

A description of the deferred payment.

