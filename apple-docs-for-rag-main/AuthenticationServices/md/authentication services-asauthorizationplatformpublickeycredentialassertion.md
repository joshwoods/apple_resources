

- Authentication Services
-  ASAuthorizationPlatformPublicKeyCredentialAssertion 

Class

# ASAuthorizationPlatformPublicKeyCredentialAssertion

A class that represents the platform credential assertion type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class ASAuthorizationPlatformPublicKeyCredentialAssertion
```

## Overview

The device creates an assertion when signing in with an existing credential. Use this class to verify the platform credential assertion when the authorization controller calls authorizationController(controller:didCompleteWithAuthorization:).

## Topics

### Creating requests

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

class ASAuthorizationPlatformPublicKeyCredentialDescriptor

An object that holds the credential.

### Instance Properties

var attachment: ASAuthorizationPublicKeyCredentialAttachment

var largeBlob: ASAuthorizationPublicKeyCredentialLargeBlobAssertionOutput?

var prf: ASAuthorizationPublicKeyCredentialPRFAssertionOutput?

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationCredential
- ASAuthorizationPublicKeyCredentialAssertion
- ASPublicKeyCredential
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

### Account authentication

protocol ASAuthorizationPublicKeyCredentialAssertion

An interface for establishing a public key-based assertion.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

A class that represents the security key credential assertion type.

protocol ASAuthorizationPublicKeyCredentialAssertionRequest

An interface for requesting a public key-based credential assertion.

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

