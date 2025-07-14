

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor

An object that holds public key credential transport information.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor
```

## Overview

This class ties together a credential and its corresponding transport types (USB, NFC, Bluetooth, or all of them).

## Topics

### Creating the descriptor

init(credentialID: Data, transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport])

Creates the object with the credential ID and the array of transports.

var transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]

The array of transport types.

struct Transport

A structure that defines the security key credential transport type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationPublicKeyCredentialDescriptor
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
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

struct ASAuthorizationPublicKeyCredentialUserVerificationPreference

A structure that defines the relying party’s user verification preference.

protocol ASAuthorizationPublicKeyCredentialDescriptor

An interface that defines the credential identifier.

class ASAuthorizationPlatformPublicKeyCredentialDescriptor

An object that holds the credential.

struct Transport

A structure that defines the security key credential transport type.

static var allSupported: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]

An array of currently supported transport types.

