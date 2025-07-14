

- Apple Pay on the Web
- ApplePayDeferredPaymentRequest
-  billingAgreement 

Instance Property

# billingAgreement

The localized billing agreement the framework displays to the user prior to payment authorization.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString billingAgreement;
```

## Discussion

This may include additional details about the cancellation period or penalties for late cancellation. This value is optional.

## See Also

### Describing a deferred payment

paymentDescription

A description of the deferred payment.

freeCancellationDate

The time zone at the destination location of the payment.

freeCancellationDateTimeZone

The time zone at the destination location of the payment.

