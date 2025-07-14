

- Authentication Services
-  ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest 

Class

# ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

The object for registering a new platform public key credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
```

## Mentioned in 

Supporting passkeys

## Overview

Create an instance of this class when registering for a new credential using platform authorization.

## Topics

### Instance Properties

var largeBlob: ASAuthorizationPublicKeyCredentialLargeBlobRegistrationInput?

var prf: ASAuthorizationPublicKeyCredentialPRFRegistrationInput?

var requestStyle: ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle

### Enumerations

enum RequestStyle

## Relationships

### Inherits From

- ASAuthorizationRequest

### Conforms To

- ASAuthorizationPublicKeyCredentialRegistrationRequest
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest
- CVarArg
- Copyable
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

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

A newly created security key credential that results from a credential registration request.

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

The object for registering a new security key credential.

