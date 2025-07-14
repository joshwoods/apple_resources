

- Apple Pay on the Web
-  ApplePayShippingMethodUpdate 

Structure

# ApplePayShippingMethodUpdate

Updated transaction details that result from a change in shipping method.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayShippingMethodUpdate {
 required ApplePayLineItem newTotal;
 sequence  newLineItems;
 sequence  newMultiTokenContexts;
 ApplePayAutomaticReloadPaymentRequest newAutomaticReloadPaymentRequest;
 ApplePayRecurringPaymentRequest newRecurringPaymentRequest;
 ApplePayDeferredPaymentRequest newDeferredPaymentRequest;
 sequence  newShippingMethods;
};
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Overview

Provide updated transaction details if the user changes the shipping method in the payment sheet. Recalculate the total for the payment, because it may change as a result of shipping method changes. The newTotal value is required.

## Topics

### Updating shipping method properties

newLineItems

An optional list of updated line items.

newTotal

The new total that results from a change in the shipping method.

newShippingMethods

An updated list of new shipping methods.

### Updating automatic reload payments

newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

### Updating multitoken or multimerchant payment

newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

### Updating recurring payments

newRecurringPaymentRequest

An updated request for a recurring payment.

### Updating deferred payments

newDeferredPaymentRequest

An updated request for a deferred payment.

## See Also

### Handling shipping method updates

onshippingmethodselected

An event handler to call when the user selects a shipping method.

completeShippingMethodSelection

Completes the selection of a shipping method with an update.

ApplePayShippingMethodSelectedEvent

An event object that contains the shipping method.

