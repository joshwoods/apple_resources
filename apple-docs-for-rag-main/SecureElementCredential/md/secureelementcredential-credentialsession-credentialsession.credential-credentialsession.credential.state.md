

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
-  CredentialSession.Credential.State 

Enumeration

# CredentialSession.Credential.State

An enumeration of possible values of a credential’s installation state.

iOS 18.1+iPadOS 18.1+

``` source
enum State
```

## Topics

### Credential states

case installationPending

The credential installation is pending but isn’t complete.

case installed(instances: [CredentialSession.Credential.InstanceInfo])

The credential installation is complete for one or more instances.

struct InstanceInfo

Information about an applet instance associated with a specific credential.

case installationFailed

The credential installation failed.

### Operators

static func == (CredentialSession.Credential.State, CredentialSession.Credential.State) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Inspecting credential state

let state: CredentialSession.Credential.State

A snapshot of the credential’s installation state.

