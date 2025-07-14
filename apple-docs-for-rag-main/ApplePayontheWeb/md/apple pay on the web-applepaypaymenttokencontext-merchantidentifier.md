

- Apple Pay on the Web
- ApplePayPaymentTokenContext
-  merchantIdentifier 

Instance Property

# merchantIdentifier

The Apply Pay merchant identifier.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString merchantIdentifier;
```

## Discussion

The merchant identifier you provide when you make an Apple Pay payment request. If you request a payment token for another merchant, use their merchant identifier, if available. Otherwise, use your own merchant identifier.

For more information about merchant identifiers, see Configuring Your Environment.

## See Also

### Specifying the merchant

merchantName

The merchant’s display name that the Apple Pay server associates with the payment token.

merchantDomain

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

externalIdentifier

An external identifier for the merchant.

