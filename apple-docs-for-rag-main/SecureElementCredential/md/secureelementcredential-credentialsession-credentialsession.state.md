

- SecureElementCredential
- CredentialSession
-  CredentialSession.State 

Enumeration

# CredentialSession.State

An enumeration of the possible states of a card session.

iOS 18.1+iPadOS 18.1+

``` source
enum State
```

## Topics

### Card session states

case management

The state for managing the credential session.

case wired(credential: CredentialSession.Credential)

The state for performing wired operations with a given credential.

case cardEmulation(credential: CredentialSession.Credential)

The state for performing card emulation with a given credential.

struct Credential

Information about a credential that a credential session retrieves from the Secure Element.

case invalid

The state of an invalid credential session.

### Comparing states

static func == (CredentialSession.State, CredentialSession.State) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Accessing the session state

var state: CredentialSession.State

The current state of the session.

