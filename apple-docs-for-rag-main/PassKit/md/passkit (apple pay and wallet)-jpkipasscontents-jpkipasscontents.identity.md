

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  JPKIPassContents.Identity 

Protocol

# JPKIPassContents.Identity

Defines the common functionality that JPKI digital identities support.

iOS 18.0+iPadOS 18.0+

``` source
protocol Identity
```

## Topics

### Data associated with the identity

associatedtype IdentityType : JPKIPassContents.Identity

The type associated with the protocol.

**Required**

func certificate(using: JPKIPassContents.AuthenticationRequest&lt;Self.IdentityType>) async throws -> JPKIPassContents.Certificate&lt;Self.IdentityType>

The certificate associated with the Identity.

**Required**

### Instance Properties

var authenticationTriesRemaining: Int

The tries remaining before the underlying credential locks itself

**Required**

### Instance Methods

func signature(for: [Data], using: JPKIPassContents.AuthenticationRequest&lt;Self.IdentityType>) async throws -> [JPKIPassContents.Signature&lt;Self.IdentityType>]

Signs the supplied array of data with the identity’s private key

**Required**

func signature(for: Data, using: JPKIPassContents.AuthenticationRequest&lt;Self.IdentityType>) async throws -> JPKIPassContents.Signature&lt;Self.IdentityType>

Signs the supplied data with the identity’s private key

**Required**

## Relationships

### Conforming Types

- JPKIPassContents.SigningIdentity
- JPKIPassContents.UserIdentity

## See Also

### Defining access to the identity passes

struct UserIdentity

The functionality for the type of user identification.

struct SigningIdentity

The authentication for signing user identification.

struct Signature

The resulting signed data and certificate you use to sign the pass.

struct Certificate

The certificate data associated with an identity document.

struct AuthenticationRequest

The user authentification request based on the generics type.

