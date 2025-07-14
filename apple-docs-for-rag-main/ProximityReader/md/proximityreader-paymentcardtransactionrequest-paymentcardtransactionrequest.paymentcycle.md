

- ProximityReader
- PaymentCardTransactionRequest
-  PaymentCardTransactionRequest.PaymentCycle 

Enumeration

# PaymentCardTransactionRequest.PaymentCycle

Values that specify the frequency of payments

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum PaymentCycle
```

## Topics

### Operators

static func == (PaymentCardTransactionRequest.PaymentCycle, PaymentCardTransactionRequest.PaymentCycle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case monthly

Payment is monthly.

case weekly

Payment is weekly.

case yearly

Payment is yearly.

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

