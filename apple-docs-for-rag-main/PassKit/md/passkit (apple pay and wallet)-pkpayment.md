

- PassKit (Apple Pay and Wallet)
-  PKPayment 

Class

# PKPayment

Represents the result of authorizing a payment request and contains payment information, encrypted in the payment token.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
class PKPayment
```

## Topics

### Working with the payment token

var token: PKPaymentToken

The encrypted payment information.

class PKPaymentToken

Contains the user’s payment credentials.

### Working with billing and shipping information

var billingContact: PKContact?

The user-selected billing address for this transaction.

var shippingContact: PKContact?

The user-selected shipping address for this transaction.

var shippingMethod: PKShippingMethod?

The user-selected shipping method for this transaction.

class PKContact

An object that encapsulates contact information needed for billing and shipping.

class PKShippingMethod

An object that defines a shipping method for delivering physical goods.

### Deprecated

var billingAddress: ABRecord?

The user-selected billing address for this transaction.

Deprecated

var shippingAddress: ABRecord?

The user-selected shipping address for this transaction.

Deprecated

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

class PKPaymentOrderDetails

Optional metadata with payment order details for the placed order.

class PKPaymentAuthorizationController

An object that presents a sheet that prompts the user to authorize a payment request.

class PKPaymentAuthorizationViewController

An object that presents a sheet that prompts the user to authorize a payment request.

