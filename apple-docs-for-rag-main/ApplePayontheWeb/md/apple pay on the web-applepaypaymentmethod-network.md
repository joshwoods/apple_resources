

- Apple Pay on the Web
- ApplePayPaymentMethod
-  network 

Instance Property

# network

A string, suitable for display, that is the name of the payment network backing the card.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString network;
```

## Discussion

The value is one of the supported networks specified in the supportedNetworks property of the ApplePayPaymentRequest.

## See Also

### Accessing payment method data

displayName

A string, suitable for display, that describes the card.

type

A string value representing the card’s type of payment.

paymentPass

The payment pass object currently selected to complete the payment.

billingContact

The billing contact associated with the card.

