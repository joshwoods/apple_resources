

- Authentication Services
-  ASAuthorizationPublicKeyCredentialParameters 

Class

# ASAuthorizationPublicKeyCredentialParameters

An object that provides required parameters for the credential during registration.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
class ASAuthorizationPublicKeyCredentialParameters
```

## Overview

This object is mainly for signing algorithm negotiation, and is only relevant for physical security keys.

## Topics

### Getting the parameters

init(algorithm: ASCOSEAlgorithmIdentifier)

Creates the object with an algorithm.

var algorithm: ASCOSEAlgorithmIdentifier

The algorithm to use for negitation between the authenticator and the relying party.

## Relationships

### Inherits From

- NSObject

### Conforms To

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

