

- Apple Pay on the Web
- ApplePayPaymentOrderDetails
-  orderTypeIdentifier 

Instance Property

# orderTypeIdentifier

An identifier for the order type associated with the order.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString orderTypeIdentifier;
```

## Discussion

This value must correspond with your signing certificate and isn’t displayed to the customer.

## See Also

### Providing order information

authenticationToken

The authentication token supplied to your web service.

orderIdentifier

A unique order identifier scoped to your order type identifier.

webServiceURL

The URL of your web service.

