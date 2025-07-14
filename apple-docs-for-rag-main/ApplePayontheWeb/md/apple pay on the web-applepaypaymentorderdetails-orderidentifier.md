

- Apple Pay on the Web
- ApplePayPaymentOrderDetails
-  orderIdentifier 

Instance Property

# orderIdentifier

A unique order identifier scoped to your order type identifier.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
required DOMString orderIdentifier;
```

## Discussion

In combination with the order type identifier, this uniquely identifies an order within the system. The framework doesn’t display this value to the customer.

## See Also

### Providing order information

authenticationToken

The authentication token supplied to your web service.

orderTypeIdentifier

An identifier for the order type associated with the order.

webServiceURL

The URL of your web service.

