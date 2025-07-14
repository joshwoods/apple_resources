

- Apple Pay on the Web
-  ApplePayPaymentMethodUpdate 

Structure

# ApplePayPaymentMethodUpdate

Updated transaction details to provide after the user changes the payment method in the payment sheet.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Desktop**

``` source
dictionary ApplePayPaymentMethodUpdate {
 required ApplePayLineItem newTotal;
 sequence  newLineItems;
 sequence  newMultiTokenContexts;
 ApplePayAutomaticReloadPaymentRequest newAutomaticReloadPaymentRequest;
 ApplePayRecurringPaymentRequest newRecurringPaymentRequest;
 ApplePayDeferredPaymentRequest newDeferredPaymentRequest;
 sequence  errors;
 sequence  newShippingMethods;
};
```

**Unsupported OS: Safari Mobile**

``` source
dictionary ApplePayPaymentMethodUpdate {
 required ApplePayLineItem newTotal;
 sequence  newLineItems;
 sequence  newMultiTokenContexts;
 ApplePayAutomaticReloadPaymentRequest newAutomaticReloadPaymentRequest;
 ApplePayRecurringPaymentRequest newRecurringPaymentRequest;
 ApplePayDeferredPaymentRequest newDeferredPaymentRequest;
 sequence  errors;
 sequence  newShippingMethods;
};
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Overview

If a user changes their payment method on the payment sheet, you respond by updating the payment request details in ApplePayPaymentMethodUpdate.

You must provide an updated total for the transaction in the `newTotal` line item. You can optionally provide updated line items if the change to the payment method changes the line items.

## Topics

### Updating payment method properties

newLineItems

An optional list of updated line items for the payment request that results from the user’s change to the payment method.

newTotal

The new total that results from the user’s change to the payment method.

errors

A list of customized errors you provide that results from the user’s change to the payment method.

newShippingMethods

The updated list of available shipping methods that results from the user’s change to the payment method.

### Updating automatic reload payments

newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

### Updating deferred payments

newDeferredPaymentRequest

An updated request for a deferred payment.

### Updating recurring payments

newRecurringPaymentRequest

An updated request for a recurring payment.

ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

### Updating multitoken or multimerchant payments

newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

## See Also

### Handling payment method updates

onpaymentmethodselected

An event handler to call when the user selects a new payment method.

completePaymentMethodSelection

Completes the selection of a payment method with an update.

ApplePayPaymentMethodSelectedEvent

An event object that contains the payment method.

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

