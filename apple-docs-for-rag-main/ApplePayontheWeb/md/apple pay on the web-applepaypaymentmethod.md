

- Apple Pay on the Web
-  ApplePayPaymentMethod 

Structure

# ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentMethod {
 DOMString displayName;
 DOMString network;
 ApplePayPaymentMethodType type;
 ApplePayPaymentPass paymentPass;
 ApplePayPaymentContact billingContact;
};
```

## Mentioned in 

Setting up the payment request API to accept Apple Pay

Apple Pay on the Web Version 10 Release Notes

## Topics

### Accessing payment method data

displayName

A string, suitable for display, that describes the card.

network

A string, suitable for display, that is the name of the payment network backing the card.

type

A string value representing the card’s type of payment.

paymentPass

The payment pass object currently selected to complete the payment.

billingContact

The billing contact associated with the card.

## See Also

### Handling payment method updates

onpaymentmethodselected

An event handler to call when the user selects a new payment method.

completePaymentMethodSelection

Completes the selection of a payment method with an update.

ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

