

- Apple Pay on the Web
- ApplePayModifier
-  paymentMethodType 

Instance Property

# paymentMethodType

The type of card the customer uses to complete the transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayPaymentMethodType paymentMethodType;
```

## Discussion

This property in the ApplePayModifier dictionary indicates the type of payment card that the ApplePayModifier applies to: `"credit"`, `"debit"`, `"prepaid"`, or `"store"`. To create a modifier that works with all payment types, don’t provide a value for the paymentMethodType.

The payment request uses the ApplePayModifier that matches the payment method that the customer chooses. For example, if the customer chooses to pay with a debit card, the payment request uses the ApplePayModifier with a paymentMethodType of `"debit"`, or a modifier that doesn’t specify any paymentMethodType.

## See Also

### Payment method type

ApplePayPaymentMethodType

A string that represents the type of the payment method.

