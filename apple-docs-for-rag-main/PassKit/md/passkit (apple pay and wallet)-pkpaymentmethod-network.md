

- PassKit (Apple Pay and Wallet)
- PKPaymentMethod
-  network 

Instance Property

# network

A string, suitable for display, that describes the payment network for the card.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var network: PKPaymentNetwork? { get }
```

## Discussion

To protect the user’s privacy, the `network` property is `nil` until after the user authenticates the purchase. You can safely access this property as soon as the system calls your delegate’s paymentAuthorizationController(_:didAuthorizePayment:completion:) method.

## See Also

### Getting the payment method’s attributes

var type: PKPaymentMethodType

A value that represents the card’s type.

enum PKPaymentMethodType

The type of cards available in Apple Pay.

var displayName: String?

A string, suitable for display, that describes the card.

var billingAddress: CNContact?

The user’s billing address.

