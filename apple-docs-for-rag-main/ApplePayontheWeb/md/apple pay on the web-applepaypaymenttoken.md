

- Apple Pay on the Web
-  ApplePayPaymentToken 

Structure

# ApplePayPaymentToken

An object that contains the user’s payment credentials.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentToken {
 required ApplePayPaymentMethod paymentMethod;
 DOMString transactionIdentifier;
 JSON paymentData;
};
```

## Overview

You access the payment token of an authorized payment request using the token property of the ApplePayPayment object.

## Topics

### Payment Token Properties

paymentMethod

Information about the card used in the transaction.

paymentData

An object containing the encrypted payment data.

transactionIdentifier

A unique identifier for this payment.

## See Also

### Payment token

token

The encrypted information for an authorized payment.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

ApplePayPaymentMethodType

A string that represents the type of the payment method.

ApplePayPaymentPass

A provisioned payment card for Apple Pay payments.

