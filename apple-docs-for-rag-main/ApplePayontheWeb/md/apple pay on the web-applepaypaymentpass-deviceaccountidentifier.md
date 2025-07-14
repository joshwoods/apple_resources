

- Apple Pay on the Web
- ApplePayPaymentPass
-  deviceAccountIdentifier 

Instance Property

# deviceAccountIdentifier

The unique identifier for the device-specific account number.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString deviceAccountIdentifier;
```

## Discussion

This number is not the account number itself. If the pass has not been provisioned, the value of this property is `nil`.

## See Also

### Account Identity

primaryAccountIdentifier

The unique identifier for the primary account number for the payment card.

primaryAccountNumberSuffix

A version of the primary account number suitable for display in your UI.

deviceAccountNumberSuffix

A version of the device account number suitable for display in your UI.

