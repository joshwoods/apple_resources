

- SecureElementCredential
- CredentialSession
- CredentialSession.PresentmentIntentAssertion
-  CredentialSession.PresentmentIntentAssertion.State 

Enumeration

# CredentialSession.PresentmentIntentAssertion.State

An enumeration of possible states of a presentment intent assertion.

iOS 18.1+iPadOS 18.1+

``` source
enum State
```

## Topics

### Assertion states

case active

The presentment intent assertion is active, offering exclusive use of the device’s contactless features.

case invalid

The presentment intent assertion is invalid, and does not provide exclusive use of contactless features.

### Operators

static func == (CredentialSession.PresentmentIntentAssertion.State, CredentialSession.PresentmentIntentAssertion.State) -> Bool

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

## See Also

### Inspecting assertion state

var state: CredentialSession.PresentmentIntentAssertion.State

The state of a presentment intent assertion, indicating whether it’s currently valid.

