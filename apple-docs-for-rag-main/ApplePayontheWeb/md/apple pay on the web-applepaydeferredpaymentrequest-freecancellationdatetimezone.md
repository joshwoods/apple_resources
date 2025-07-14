

- Apple Pay on the Web
- ApplePayDeferredPaymentRequest
-  freeCancellationDateTimeZone 

Instance Property

# freeCancellationDateTimeZone

The time zone at the destination location of the payment.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString freeCancellationDateTimeZone;
```

## Discussion

For a hotel booking, for example, this refers to the local time zone of the hotel. On the payment sheet, this is the time zone the framework uses to format the cancellation date. If you set the `freeCancellationDateTimeZone` date, you need to set freeCancellationDate as well.

## See Also

### Describing a deferred payment

billingAgreement

The localized billing agreement the framework displays to the user prior to payment authorization.

paymentDescription

A description of the deferred payment.

freeCancellationDate

The time zone at the destination location of the payment.

