

- SecureElementCredential
- CredentialSession
-  CredentialSession.Credential 

Structure

# CredentialSession.Credential

Information about a credential that a credential session retrieves from the Secure Element.

iOS 18.1+iPadOS 18.1+

``` source
struct Credential
```

## Mentioned in 

Accessing and using secure element credentials

## Overview

A credential is an abstraction of the cryptographic elements of your applet bundle installed in the Secure Element. You perform this installation with provisionCredential(configurationUUID:name:), which retrieves the applet bundle you registered with the Apple Business Register, installs it in the Secure Element, and returns a `Credential` instance.

`Credential` objects are snapshots of credential data at the time the listCredentials() method loads them. To ensure up-to-date metadata, reload credentials with that same method.

## Topics

### Identifying a credential

let identifier: UUID

A unique identifier for the credential.

### Getting a display name

let name: String

A readable name for the credential.

### Inspecting credential state

let state: CredentialSession.Credential.State

A snapshot of the credential’s installation state.

enum State

An enumeration of possible values of a credential’s installation state.

### Hashing

func hash(into: inout Hasher)

Hashes the essential components of the value by feeding them into the given hasher.

### Comparing credentials

static func == (CredentialSession.Credential, CredentialSession.Credential) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Structures

struct InstanceInfo

Information about an applet instance associated with a specific credential.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Accessing credentials

func listCredentials() async throws -> [CredentialSession.Credential]

Retrieves a list of of credentials to which the app has access rights.

