

- Authentication Services
-  ASAuthorizationPublicKeyCredentialRegistration 

Protocol

# ASAuthorizationPublicKeyCredentialRegistration

An interface that credential registration requests adhere to.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
protocol ASAuthorizationPublicKeyCredentialRegistration : ASPublicKeyCredential
```

## Topics

### Getting attestation information

var rawAttestationObject: Data?

A data object that contains the returned attestation.

**Required**

## Relationships

### Inherits From

- ASAuthorizationCredential
- ASPublicKeyCredential
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialRegistration
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

## See Also

### Account registration

class ASAuthorizationPlatformPublicKeyCredentialRegistration

A newly created platform credential that results from a credential registration request.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistration

A newly created security key credential that results from a credential registration request.

protocol ASAuthorizationPublicKeyCredentialRegistrationRequest

An interface that defines properties for a credential registration request.

class ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

The object for registering a new platform public key credential.

class ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

The object for registering a new security key credential.

