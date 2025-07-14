

- Apple Pay on the Web
-  ApplePayAutomaticReloadPaymentRequest 

Structure

# ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayAutomaticReloadPaymentRequest {
 required DOMString paymentDescription;
 required ApplePayLineItem automaticReloadBilling;
 DOMString billingAgreement;
 required DOMString managementURL;
 DOMString tokenNotificationURL;
};
```

## Overview

Important

You must include the automaticReloadPaymentRequest property in the ApplePayPaymentRequest object to set up an automatic reload payment.

Use an ApplePayAutomaticReloadPaymentRequest object to provide the user with payment details and a way to manage payment methods for an automatic reload payment. You can optionally display a billing agreement and set up merchant token life-cycle notifications for the request. For more information about the merchant token life-cycle notifications, see Apple Pay Merchant Token Management API.

Apple Pay issues an Apple Pay Merchant Token if the user’s payment network supports merchant-specific payment tokens. Otherwise, Apple Pay issues a device token for the payment request.

## Topics

### Describing an automatic reload payment

paymentDescription

A description of the automatic reload payment that Apple Pay displays in the payment sheet.

billingAgreement

A localized billing agreement that the payment sheet displays to the user before the user authorizes the payment.

### Setting the payment summary items

automaticReloadBilling

A line item that contains the reload amount and balance threshold for the automatic reload payment.

ApplePayLineItem

A line item in a payment request—for example, total, tax, discount, or grand total.

### Receiving payment token notifications

tokenNotificationURL

A URL you provide to receive life-cycle notifications from the Apple Pay servers about the Apple Pay merchant token for the recurring payment.

### Managing the automatic reload payment

managementURL

A URL to a web page where the user can update or delete the payment method for the automatic reload payment.

## See Also

### Requesting automatic reload payments

automaticReloadPaymentRequest

A property that requests an automatic reload payment, such as a store card top-up.

