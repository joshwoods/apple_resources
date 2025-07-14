

- Apple Pay on the Web
- ApplePayPaymentOrderDetails
-  webServiceURL 

Instance Property

# webServiceURL

The URL of your web service.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString webServiceURL;
```

## Discussion

The URL for your web service needs to begin with `https://`; for example, `https://example.com`.

## See Also

### Providing order information

authenticationToken

The authentication token supplied to your web service.

orderIdentifier

A unique order identifier scoped to your order type identifier.

orderTypeIdentifier

An identifier for the order type associated with the order.

