

- Apple Pay on the Web
-  ApplePayPaymentPass 

Structure

# ApplePayPaymentPass

A provisioned payment card for Apple Pay payments.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentPass {
 required DOMString primaryAccountIdentifier;
 required DOMString primaryAccountNumberSuffix;
 DOMString deviceAccountIdentifier;
 DOMString deviceAccountNumberSuffix;
 required ApplePayPaymentPassActivationState activationState;
};
```

## Overview

Payment pass information is populated only for cobranded or private label cards, for specially registered websites.

## Topics

### Account Identity

primaryAccountIdentifier

The unique identifier for the primary account number for the payment card.

primaryAccountNumberSuffix

A version of the primary account number suitable for display in your UI.

deviceAccountIdentifier

The unique identifier for the device-specific account number.

deviceAccountNumberSuffix

A version of the device account number suitable for display in your UI.

### Activation State

activationState

The activation state of the pass.

ApplePayPaymentPassActivationState

Payment pass activation states.

## See Also

### Payment token

token

The encrypted information for an authorized payment.

ApplePayPaymentToken

An object that contains the user’s payment credentials.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

ApplePayPaymentMethodType

A string that represents the type of the payment method.

