

- Apple Pay on the Web
-  ApplePayShippingContactUpdate 

Structure

# ApplePayShippingContactUpdate

Updated transaction details that result from a change in shipping contact, including any errors.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Desktop**

``` source
dictionary ApplePayShippingContactUpdate {
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
dictionary ApplePayShippingContactUpdate {
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

You must provide an updated total after shipping contact information changes. You can optionally provide a list of errors, updated shipping methods, or updated line items.

The system assumes the shipping contact update is successful if you don’t provide any `errors` in the ApplePayShippingContactUpdate.

## Topics

### Updating shipping contact properties

errors

A list of custom errors to display on the payment sheet.

newLineItems

An optional list of updated line items.

newShippingMethods

A list of shipping methods that are available to the updated shipping contact.

newTotal

The new total that results from a change in the shipping contact.

### Updating recurrring payments

newRecurringPaymentRequest

An updated request for a recurring payment.

ApplePayRecurringPaymentRequest

A dictionary that represents a request to set up a recurring payment, typically a subscription.

### Updating deferred payments

newDeferredPaymentRequest

An updated request for a deferred payment.

### Updating automatic reload payments

newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

ApplePayAutomaticReloadPaymentRequest

A dictionary that represents a request to set up an automatic reload payment, such as a store card top-up or a prepaid account.

### Updating multitoken or multimerchant payments

newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

ApplePayPaymentTokenContext

A dictionary that defines the context for a single payment token in a payment request for multimerchant payments.

## See Also

### Handling shipping contact updates

onshippingcontactselected

An event handler to call when the user selects a shipping contact in the payment sheet.

completeShippingContactSelection

Completes the selection of a shipping contact with an update.

ApplePayShippingContactSelectedEvent

An event object that contains the shipping address the user selects.

