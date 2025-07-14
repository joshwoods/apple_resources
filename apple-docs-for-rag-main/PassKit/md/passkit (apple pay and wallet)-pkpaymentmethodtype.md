

- PassKit (Apple Pay and Wallet)
-  PKPaymentMethodType 

Enumeration

# PKPaymentMethodType

The type of cards available in Apple Pay.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPaymentMethodType
```

## Topics

### Payment Method Type Constants

case unknown

The card’s type is unknown.

case debit

A debit card.

case eMoney

An electronic money card.

case credit

A credit card.

case prepaid

A prepaid card.

case store

A store card.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the payment method’s attributes

var type: PKPaymentMethodType

A value that represents the card’s type.

var displayName: String?

A string, suitable for display, that describes the card.

var network: PKPaymentNetwork?

A string, suitable for display, that describes the payment network for the card.

var billingAddress: CNContact?

The user’s billing address.

