

- Apple Pay on the Web
- ApplePayPaymentPass
-  primaryAccountNumberSuffix 

Instance Property

# primaryAccountNumberSuffix

A version of the primary account number suitable for display in your UI.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString primaryAccountNumberSuffix;
```

## Discussion

Note that this value is typically the last four or five digits of the account number, but the number of digits can vary by issuer. This value is not related to the value of the primaryAccountIdentifier value.

## See Also

### Account Identity

primaryAccountIdentifier

The unique identifier for the primary account number for the payment card.

deviceAccountIdentifier

The unique identifier for the device-specific account number.

deviceAccountNumberSuffix

A version of the device account number suitable for display in your UI.

