

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
-  CredentialSession.Credential.InstanceInfo 

Structure

# CredentialSession.Credential.InstanceInfo

Information about an applet instance associated with a specific credential.

iOS 18.1+iPadOS 18.1+

``` source
struct InstanceInfo
```

## Topics

### Inspecting instance identifiers

let instanceAID: Data

The unique identifier for the applet instance.

let packageAID: Data

The unique identifier of the package you use to install the instance.

let moduleAID: Data

The module identifier of the package with which this instance is associated.

### Creating a secure channel

let securityDomainAID: Data

The unique identifier of the security domain you use to install the instance.

let securityDomainKeyInfo: Data

A data blob which contains the security domain On-Board Generated Key (OBGK).

### Inspecting applet instance state

let lifeCycleState: Data

Information about the state of the applet instance.

### Operators

static func == (CredentialSession.Credential.InstanceInfo, CredentialSession.Credential.InstanceInfo) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var securityDomainCounter: Int

The authentication counter of the security domain. Fetches the latest counter from the remote hardware.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Credential states

case installationPending

The credential installation is pending but isn’t complete.

case installed(instances: [CredentialSession.Credential.InstanceInfo])

The credential installation is complete for one or more instances.

case installationFailed

The credential installation failed.

