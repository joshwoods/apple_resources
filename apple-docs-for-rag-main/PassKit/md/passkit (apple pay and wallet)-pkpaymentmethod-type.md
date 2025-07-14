

- PassKit (Apple Pay and Wallet)
- PKPaymentMethod
-  type 

Instance Property

# type

A value that represents the card’s type.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var type: PKPaymentMethodType { get }
```

## Discussion

For a list of possible card types, see PKPaymentMethodType.

Note

Some older cards might not have card type information. Those cards have the value PKPaymentMethodType.unknown.

## See Also

### Getting the payment method’s attributes

enum PKPaymentMethodType

The type of cards available in Apple Pay.

var displayName: String?

A string, suitable for display, that describes the card.

var network: PKPaymentNetwork?

A string, suitable for display, that describes the payment network for the card.

var billingAddress: CNContact?

The user’s billing address.

