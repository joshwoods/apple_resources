

- PassKit (Apple Pay and Wallet)
-  PKPaymentOrderDetails 

Class

# PKPaymentOrderDetails

Optional metadata with payment order details for the placed order.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class PKPaymentOrderDetails
```

## Overview

The device only retreives metadata if the status is `PKPaymentAuthorizationStatusSuccess`.

## Topics

### Creating payment order details

init(orderTypeIdentifier: String, orderIdentifier: String, webServiceURL: URL, authenticationToken: String)

Initializes a payment order details object with the identifier, web service URL, and authentication token you provide.

### Identifying and authenticating the order

var authenticationToken: String

The authentification token supplied to your web service.

var orderIdentifier: String

A unique order identifier scoped to your order type identifier.

var orderTypeIdentifier: String

An identifier for the order type associated with the order.

var webServiceURL: URL

The URL for your web service.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Payment sheet interactions and authorization

class PKPaymentAuthorizationResult

An object that reports the status code and errors for a payment authorization request.

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPayment

Represents the result of authorizing a payment request and contains payment information, encrypted in the payment token.

