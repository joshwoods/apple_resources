

- Authentication Services
-  ASAuthorizationPlatformPublicKeyCredentialRegistration 

Class

# ASAuthorizationPlatformPublicKeyCredentialRegistration

A newly created platform credential that results from a credential registration request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class ASAuthorizationPlatformPublicKeyCredentialRegistration
```

## Mentioned in 

Supporting passkeys

## Overview

Use this class to verify a successful platform authorization request in authorizationController(controller:didCompleteWithAuthorization:).

## Topics

### Instance Properties

var attachment: ASAuthorizationPublicKeyCredentialAttachment

var largeBlob: ASAuthorizationPublicKeyCredentialLargeBlobRegistrationOutput?

var prf: ASAuthorizationPublicKeyCredentialPRFRegistrationOutput?

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASAuthorizationCredential
- ASAuthorizationPublicKeyCredentialRegistration
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

### Account registration

protocol ASAuthorizationPublicKeyCredentialRegistration

An interface that credential registration requests adhere to.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

A newly created security key credential that results from a credential registration request.

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

The object for registering a new platform public key credential.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

The object for registering a new security key credential.

