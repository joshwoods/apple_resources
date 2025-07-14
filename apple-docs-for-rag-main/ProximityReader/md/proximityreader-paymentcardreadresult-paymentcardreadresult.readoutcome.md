

- ProximityReader
- PaymentCardReadResult
-  PaymentCardReadResult.ReadOutcome 

Enumeration

# PaymentCardReadResult.ReadOutcome

Values that describe the outcome of a read request.

iOS 16.4+iPadOS 16.4+Mac Catalyst 17.0+

``` source
enum ReadOutcome
```

## Topics

### Getting the read outcome

case success

The read was successful.

case failure

The read failed somehow, the card data may not contain all requested tags.

case cardDeclined

The card declined this transaction.

### Operators

static func == (PaymentCardReadResult.ReadOutcome, PaymentCardReadResult.ReadOutcome) -> Bool

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

### Checking the read outcome

let outcome: PaymentCardReadResult.ReadOutcome

The outcome of the transaction.

