

- Apple Pay on the Web
-  ApplePayDeferredPaymentRequest 

Structure

# ApplePayDeferredPaymentRequest

A dictionary that represents a request to set up a deferred payment, such as a hotel booking or a pre-order.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayDeferredPaymentRequest {
 DOMString billingAgreement;
 required ApplePayLineItem deferredBilling;
 Date freeCancellationDate;
 DOMString freeCancellationDateTimeZone;
 required DOMString managementURL;
 required DOMString paymentDescription;
 DOMString tokenNotificationURL;
};
```

## Topics

### Describing a deferred payment

billingAgreement

The localized billing agreement the framework displays to the user prior to payment authorization.

paymentDescription

A description of the deferred payment.

freeCancellationDate

The time zone at the destination location of the payment.

freeCancellationDateTimeZone

The time zone at the destination location of the payment.

### Setting payment summary items

deferredBilling

A dictionary that contains details about the deferred payment.

### Managing payment tokens

managementURL

A URL that links to a page on your web site where the user can manage the payment method for the deferred payment, including deleting it.

tokenNotificationURL

A URL to receive life-cycle notifications for the merchant-specific payment token the system issues for the request, if applicable.

## See Also

### Apple Pay payment request

ApplePayPaymentRequest

A request for payment, which includes information about payment-processing capabilities, the payment amount, and shipping information.

