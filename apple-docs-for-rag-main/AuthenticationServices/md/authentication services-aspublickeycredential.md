

- Authentication Services
-  ASPublicKeyCredential 

Protocol

# ASPublicKeyCredential

An interface that defines the properties of the public key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
protocol ASPublicKeyCredential : ASAuthorizationCredential
```

## Topics

### Getting the properties

var credentialID: Data

An identifier that the authenticator generates during registration to uniquely identify a specific credential.

**Required**

var rawClientDataJSON: Data

Raw data that contains a JSON-compatible encoding of the client data.

**Required**

## Relationships

### Inherits From

- ASAuthorizationCredential
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Inherited By

- ASAuthorizationPublicKeyCredentialAssertion
- ASAuthorizationPublicKeyCredentialRegistration

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialAssertion
- ASAuthorizationPlatformPublicKeyCredentialRegistration
- ASAuthorizationSecurityKeyPublicKeyCredentialAssertion
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

## See Also

### Request configuration

class ASAuthorizationPublicKeyCredentialParameters

An object that provides required parameters for the credential during registration.

struct ASCOSEAlgorithmIdentifier

An identifier for the algorithm that a credential’s key pair uses.

struct ASCOSEEllipticCurveIdentifier

A structure that contains the elliptic curve identifier.

struct ASAuthorizationPublicKeyCredentialAttestationKind

A structure that defines the types of attestations a developer can request.

struct ASAuthorizationPublicKeyCredentialResidentKeyPreference

A structure that specifies the relying party’s preference for resident key storage.

struct ASAuthorizationPublicKeyCredentialUserVerificationPreference

A structure that defines the relying party’s user verification preference.

protocol ASAuthorizationPublicKeyCredentialDescriptor

An interface that defines the credential identifier.

class ASAuthorizationPlatformPublicKeyCredentialDescriptor

An object that holds the credential.

class ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor

An object that holds public key credential transport information.

struct Transport

A structure that defines the security key credential transport type.

static var allSupported: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]

An array of currently supported transport types.

