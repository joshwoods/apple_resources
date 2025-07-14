

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest
```

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

## Overview

Use this class to sign in with an existing credential on a security key.

## Topics

### Getting the properties

var allowedCredentials: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor]

An array of allowed credentials.

### Instance Properties

var appID: String?

## Relationships

### Inherits From

- ASAuthorizationRequest

### Conforms To

- ASAuthorizationPublicKeyCredentialAssertionRequest
- ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialAssertionRequest
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

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

