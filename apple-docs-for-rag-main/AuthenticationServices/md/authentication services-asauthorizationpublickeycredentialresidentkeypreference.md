

- Authentication Services
-  ASAuthorizationPublicKeyCredentialResidentKeyPreference 

Structure

# ASAuthorizationPublicKeyCredentialResidentKeyPreference

A structure that specifies the relying party’s preference for resident key storage.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
struct ASAuthorizationPublicKeyCredentialResidentKeyPreference
```

## Topics

### Creating the preference

init(String)

Creates the object with a preference.

init(rawValue: String)

Creates the object with a preference.

### Getting preferences

static let discouraged: ASAuthorizationPublicKeyCredentialResidentKeyPreference

The preference for the device not to store the resident key.

static let preferred: ASAuthorizationPublicKeyCredentialResidentKeyPreference

The preference for the device to store the resident key.

static let required: ASAuthorizationPublicKeyCredentialResidentKeyPreference

The device must store the resident key.

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

