

- Authentication Services
-  ASAuthorizationPlatformPublicKeyCredentialAssertionRequest 

Class

# ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest
```

## Mentioned in 

Supporting passkeys

## Overview

Use this class to sign in with an existing credential that the system stores in iCloud Keychain.

## Topics

### Getting the properties

var allowedCredentials: [ASAuthorizationPlatformPublicKeyCredentialDescriptor]

The array of allowed credentials.

### Instance Properties

var largeBlob: ASAuthorizationPublicKeyCredentialLargeBlobAssertionInput?

var prf: ASAuthorizationPublicKeyCredentialPRFAssertionInput?

var prf: __ASAuthorizationPublicKeyCredentialPRFAssertionInput?

## Relationships

### Inherits From

- ASAuthorizationRequest

### Conforms To

- ASAuthorizationPublicKeyCredentialAssertionRequest
- ASAuthorizationWebBrowserExternallyAuthenticatableRequest
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest
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

### Account authentication

protocol ASAuthorizationPublicKeyCredentialAssertion

An interface for establishing a public key-based assertion.

class ASAuthorizationPlatformPublicKeyCredentialAssertion

A class that represents the platform credential assertion type.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

A class that represents the security key credential assertion type.

protocol ASAuthorizationPublicKeyCredentialAssertionRequest

An interface for requesting a public key-based credential assertion.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

