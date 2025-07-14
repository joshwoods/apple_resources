

- PassKit (Apple Pay and Wallet)
- PKPaymentMethod
-  displayName 

Instance Property

# displayName

A string, suitable for display, that describes the card.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var displayName: String? { get }
```

## Discussion

The display name enables a user to recognize a particular card from a list of cards.

For debit and credit cards, the display name often includes the card brand and the last four digits of the credit card number when available, for example: `“Visa 1233”`, `“MasterCard 5678”`, `“AmEx 9876”`. For Apple Pay Cash cards, the display name is `“Apple Pay Cash”`. However, there is no standard format for the display name’s content.

To protect the user’s privacy, Apple Pay sets the display name only after the user authorizes the purchase. You can safely access this property as soon as the system calls your delegate’s paymentAuthorizationController(_:didAuthorizePayment:completion:) method.

## See Also

### Getting the payment method’s attributes

var type: PKPaymentMethodType

A value that represents the card’s type.

enum PKPaymentMethodType

The type of cards available in Apple Pay.

var network: PKPaymentNetwork?

A string, suitable for display, that describes the payment network for the card.

var billingAddress: CNContact?

The user’s billing address.

