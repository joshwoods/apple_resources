

- ProximityReader
- PaymentCardReadResult
-  PaymentCardReadResult.CardExpirationState 

Enumeration

# PaymentCardReadResult.CardExpirationState

Values that describe the expiration state of the card that the system read.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
enum CardExpirationState
```

## Topics

### Operators

static func == (PaymentCardReadResult.CardExpirationState, PaymentCardReadResult.CardExpirationState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case expired

The card is expired.

case invalid

The card expiration date is invalid.

case notExpired

The card is valid.

case unknown

The card expiration date is not available.

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

