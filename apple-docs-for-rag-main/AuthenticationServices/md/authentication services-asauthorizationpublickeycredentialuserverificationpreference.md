

- Authentication Services
-  ASAuthorizationPublicKeyCredentialUserVerificationPreference 

Structure

# ASAuthorizationPublicKeyCredentialUserVerificationPreference

A structure that defines the relying party’s user verification preference.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
struct ASAuthorizationPublicKeyCredentialUserVerificationPreference
```

## Topics

### Creating the preference

init(String)

Creates the object with a preference.

init(rawValue: String)

Creates the object with a preference.

### Getting preferences

static let discouraged: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party discourages user verification.

static let preferred: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party prefers user verification.

static let required: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party requires user verification.

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

struct ASAuthorizationPublicKeyCredentialAttestationKind

A structure that defines the types of attestations a developer can request.

struct ASAuthorizationPublicKeyCredentialResidentKeyPreference

A structure that specifies the relying party’s preference for resident key storage.

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

