

- Apple Pay on the Web
-  ApplePayPaymentOrderDetails 

Structure

# ApplePayPaymentOrderDetails

A dictionary that contains metadata related to an order.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentOrderDetails {
 required DOMString orderTypeIdentifier;
 required DOMString orderIdentifier;
 required DOMString webServiceURL;
 required DOMString authenticationToken;
};
```

## Topics

### Providing order information

authenticationToken

The authentication token supplied to your web service.

orderIdentifier

A unique order identifier scoped to your order type identifier.

orderTypeIdentifier

An identifier for the order type associated with the order.

webServiceURL

The URL of your web service.

## See Also

### Providing order details

orderDetails

Optional metadata for an order that the customer placed using this payment method.

