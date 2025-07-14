

- App Intents
- IntentPaymentMethod
-  IntentPaymentMethod.PaymentType 

Enumeration

# IntentPaymentMethod.PaymentType

Constants that describe the available payment options, such as credit cards or bank accounts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum PaymentType
```

## Topics

### Getting the payment options

case applePay

case brokerage

case checking

case credit

case debit

case prepaid

case savings

case store

case unknown

### Operators

static func == (IntentPaymentMethod.PaymentType, IntentPaymentMethod.PaymentType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the payment details

var paymentType: IntentPaymentMethod.PaymentType

The kind of payment method, such as a credit card or bank account

var name: String?

The user-visible name of the payment method

var identificationHint: String?

A hint making it easier for the user to identify the payment method among others of similar name or type, such as the last several digits of a credit card number

var icon: DisplayRepresentation.Image?

The icon or image representing this payment method

