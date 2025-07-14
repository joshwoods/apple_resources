

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialRegistration 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

A newly created security key credential that results from a credential registration request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialRegistration
```

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

## Overview

Use this class to verify a successful security key authorization request in authorizationController(controller:didCompleteWithAuthorization:).

## Topics

### Instance Properties

var transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]

An array of transport types.

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

class ASAuthorizationPlatformPublicKeyCredentialRegistration

A newly created platform credential that results from a credential registration request.

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

The object for registering a new platform public key credential.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

The object for registering a new security key credential.

