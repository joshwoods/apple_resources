

- Apple Pay on the Web
-  ApplePayCouponCodeUpdate 

Structure

# ApplePayCouponCodeUpdate

A dictionary that contains the updated transaction details for responding to a coupon changed event.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Mobile**

``` source
dictionary ApplePayCouponCodeUpdate {
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

**Unsupported OS: Safari Desktop**

``` source
dictionary ApplePayCouponCodeUpdate {
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

Apple Pay on the Web Version 12 Release Notes

## Topics

### Setting updated transaction details

newLineItems

The list of updated line items incorporating the coupon code update.

newShippingMethods

The list of available shipping methods.

newTotal

The updated total resulting from the coupon code update.

errors

A list of errors resulting from the coupon code update.

### Updating automatic reload payments

newAutomaticReloadPaymentRequest

An updated request for an automatic reload payment.

### Updating deferred payments

newDeferredPaymentRequest

An updated request for a deferred payment.

### Updating recurring payments

newRecurringPaymentRequest

An updated request for a recurring payment.

### Updating multi-token or multi-merchant payments

newMultiTokenContexts

An array of updated multitoken contexts for a multimerchant payment request.

## See Also

### Handling coupons

oncouponcodechanged

An event handler called by the system when the user enters or updates a coupon code.

completeCouponCodeChange

Completes the entry of a coupon code with an update.

ApplePayCouponCodeChangedEvent

An event object that contains the coupon code entered by the user.

