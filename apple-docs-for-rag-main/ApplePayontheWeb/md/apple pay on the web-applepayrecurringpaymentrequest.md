

- Apple Pay on the Web
-  ApplePayRecurringPaymentRequest 

Structure

# ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayRecurringPaymentRequest {
 required DOMString paymentDescription;
 required ApplePayLineItem regularBilling;
 ApplePayLineItem trialBilling;
 DOMString billingAgreement;
 required DOMString managementURL;
 DOMString tokenNotificationURL;
};
```

## Overview

Important

You must include the recurringPaymentRequest property in the ApplePayPaymentRequest object to specify a request for a recurring payment.

Use an ApplePayRecurringPaymentRequest object to provide the user with payment details and a way to manage payment methods for a recurring payment. You can optionally display a billing agreement and set up merchant token life-cycle notifications for the request.

For more information about the merchant token life-cycle notifications, see Apple Pay Merchant Token Management API.

## Topics

### Describing the recurring payment

paymentDescription

A description of the recurring payment that Apple Pay displays to the user in the payment sheet.

billingAgreement

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

### Setting the payment summary items

regularBilling

The regular billing cycle for the recurring payment, including start and end dates, an interval, and an interval count.

trialBilling

The trial billing cycle for the recurring payment.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

### Receiving payment token notifications

tokenNotificationURL

A URL you provide for receiving life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the recurring payment.

### Managing the recurring payment

managementURL

A URL to a web page where the user can update or delete the payment method for the recurring payment.

## See Also

### Requesting recurring payments

recurringPaymentRequest

A property that requests a recurring payment, typically a subscription.

