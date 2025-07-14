

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

The object for registering a new security key credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest
```

## Overview

Create an instance of this class when registering for a new credential using security key authorization.

## Topics

### Getting the properties

var credentialParameters: [ASAuthorizationPublicKeyCredentialParameters]

An array of parameters for the credential.

var excludedCredentials: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor]

An array of excluded parameters for the credential.

var residentKeyPreference: ASAuthorizationPublicKeyCredentialResidentKeyPreference

The preference that indicates where the resident key resides.

## Relationships

### Inherits From

- ASAuthorizationRequest

### Conforms To

- ASAuthorizationPublicKeyCredentialRegistrationRequest
- ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialRegistrationRequest
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

class ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

The object for registering a new platform public key credential.

