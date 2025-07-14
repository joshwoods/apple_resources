

- ProximityReader
- PaymentCardReadResult
-  PaymentCardReadResult.CardEffectiveState 

Enumeration

# PaymentCardReadResult.CardEffectiveState

Values that describe the effective state of the card that was read.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
enum CardEffectiveState
```

## Topics

### Operators

static func == (PaymentCardReadResult.CardEffectiveState, PaymentCardReadResult.CardEffectiveState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case active

The card is active.

case inactive

The card is inactive.

case invalid

The card effective state is invalid.

case unknown

The card effective state is not available.

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

