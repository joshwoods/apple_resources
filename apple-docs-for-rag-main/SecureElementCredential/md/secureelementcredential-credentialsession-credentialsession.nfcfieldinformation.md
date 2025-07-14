

- SecureElementCredential
- CredentialSession
-  CredentialSession.NFCFieldInformation 

Enumeration

# CredentialSession.NFCFieldInformation

The state of an NFC RF field.

iOS 18.1+iPadOS 18.1+

``` source
enum NFCFieldInformation
```

## Topics

### Field states

case fieldAbsent

No NFC reader RF field is present.

case fieldPresent

An NFC reader’s RF field is present.

### Operators

static func == (CredentialSession.NFCFieldInformation, CredentialSession.NFCFieldInformation) -> Bool

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

### NFC field events

case fieldStateChanged(info: CredentialSession.NFCFieldInformation)

The state of the NFC RF field changed during card emulation.

