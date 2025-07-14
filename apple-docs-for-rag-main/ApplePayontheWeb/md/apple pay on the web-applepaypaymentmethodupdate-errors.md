

- Apple Pay on the Web
- ApplePayPaymentMethodUpdate
-  errors 

Instance Property

# errors

A list of customized errors you provide that results from the user’s change to the payment method.

Safari Desktop 10.0+Safari Mobile 10.0+

**Unsupported OS: Safari Mobile**

``` source
sequence  errors;
```

**Unsupported OS: Safari Desktop**

``` source
sequence  errors;
```

## Discussion

List the errors in order of importance.

For information on the possible errors, see ApplePayError.

## See Also

### Updating payment method properties

newLineItems

An optional list of updated line items for the payment request that results from the user’s change to the payment method.

newTotal

The new total that results from the user’s change to the payment method.

newShippingMethods

The updated list of available shipping methods that results from the user’s change to the payment method.

