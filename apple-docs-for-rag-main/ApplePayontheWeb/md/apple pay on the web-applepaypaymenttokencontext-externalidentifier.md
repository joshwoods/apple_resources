

- Apple Pay on the Web
- ApplePayPaymentTokenContext
-  externalIdentifier 

Instance Property

# externalIdentifier

An external identifier for the merchant.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString externalIdentifier;
```

## Discussion

An external identifier for the merchant that the developer provides. If you request a payment token for another merchant, always use the same external identifier for that merchant on your website.

## See Also

### Specifying the merchant

merchantIdentifier

The Apply Pay merchant identifier.

merchantName

The merchant’s display name that the Apple Pay server associates with the payment token.

merchantDomain

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

