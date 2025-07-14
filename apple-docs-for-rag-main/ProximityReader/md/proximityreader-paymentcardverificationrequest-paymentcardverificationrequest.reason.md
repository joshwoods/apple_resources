

- ProximityReader
- PaymentCardVerificationRequest
-  PaymentCardVerificationRequest.Reason 

Enumeration

# PaymentCardVerificationRequest.Reason

The reason for the verification request.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
enum Reason
```

## Topics

### Getting the verification reason

case lookUp

Verify the payment card to look up a past transaction.

case openTab

Check if the card is valid.

case saveCard

Save the card information for later.

case other

Verify the card information.

### Operators

static func == (PaymentCardVerificationRequest.Reason, PaymentCardVerificationRequest.Reason) -> Bool

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

### Getting the request details

let currencyCode: String

The ISO 4217 code that indicates the currency type.

let verificationReason: PaymentCardVerificationRequest.Reason

The reason you asked to verify someone’s card.

