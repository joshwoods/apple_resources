

- Authentication Services
-  ASAuthorizationPublicKeyCredentialAttestationKind 

Structure

# ASAuthorizationPublicKeyCredentialAttestationKind

A structure that defines the types of attestations a developer can request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct ASAuthorizationPublicKeyCredentialAttestationKind
```

## Topics

### Creating the attestation type

init(String)

Creates the object with an attestation type.

init(rawValue: String)

Creates the object with an attestation type.

### Getting attestation types

static let none: ASAuthorizationPublicKeyCredentialAttestationKind

An attestation kind of none.

static let direct: ASAuthorizationPublicKeyCredentialAttestationKind

An attestation kind of direct.

static let enterprise: ASAuthorizationPublicKeyCredentialAttestationKind

An attestation kind of enterprise.

static let indirect: ASAuthorizationPublicKeyCredentialAttestationKind

An attestation kind of indirect.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Request configuration

protocol ASPublicKeyCredential

An interface that defines the properties of the public key.

class ASAuthorizationPublicKeyCredentialParameters

An object that provides required parameters for the credential during registration.

struct ASCOSEAlgorithmIdentifier

An identifier for the algorithm that a credential’s key pair uses.

struct ASCOSEEllipticCurveIdentifier

A structure that contains the elliptic curve identifier.

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

