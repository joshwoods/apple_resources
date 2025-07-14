

- PassKit (Apple Pay and Wallet)
- PKPaymentOrderDetails
-  orderIdentifier 

Instance Property

# orderIdentifier

A unique order identifier scoped to your order type identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var orderIdentifier: String { get set }
```

## See Also

### Identifying and authenticating the order

var authenticationToken: String

The authentification token supplied to your web service.

var orderTypeIdentifier: String

An identifier for the order type associated with the order.

var webServiceURL: URL

The URL for your web service.

