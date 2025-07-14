

- PassKit (Apple Pay and Wallet)
- PKPaymentMethod
-  billingAddress 

Instance Property

# billingAddress

The user’s billing address.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var billingAddress: CNContact? { get }
```

## Discussion

For privacy, PassKit partially redacts the user’s billing address. PassKit populates this property only when the app doesn’t request a shipping address.

## See Also

### Getting the payment method’s attributes

var type: PKPaymentMethodType

A value that represents the card’s type.

enum PKPaymentMethodType

The type of cards available in Apple Pay.

var displayName: String?

A string, suitable for display, that describes the card.

var network: PKPaymentNetwork?

A string, suitable for display, that describes the payment network for the card.

