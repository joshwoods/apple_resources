

- Apple Pay on the Web
-  PaymentMethodChangeEvent 

Class

# PaymentMethodChangeEvent

The Apple Pay extensions to the Payment Request payment change event.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
interface PaymentMethodChangeEvent
```

## Mentioned in 

Setting up the payment request API to accept Apple Pay

Apple Pay on the Web Version 12 Release Notes

## Overview

The Payment Request API sends a PaymentMethodChangeEvent when the user updates transaction information. For more information on PaymentMethodChangeEvent, see the W3C Payment Request API.

### Apple Pay Events

Custom Apple Pay events include information in the methodDetails attribute of the change event:

ApplePayCouponCodeDetails  
A dictionary type that indicates the user updated the coupon code.

ApplePayPaymentMethod  
A dictionary type that indicates that the user changed the payment method.

## Topics

### Change Information

methodName

The identifier for the payment method to use for the transaction.

methodDetails

A dictionary that contains the details of the change.

## See Also

### Related Documentation

ApplePayPaymentMethod

A dictionary that describes an Apple Pay payment method.

### Respond to payment request change events

ApplePayCouponCodeDetails

A dictionary that contains the updated coupon code.

