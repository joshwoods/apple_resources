

- Authentication Services
-  ASAuthorizationSecurityKeyPublicKeyCredentialAssertion 

Class

# ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

A class that represents the security key credential assertion type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class ASAuthorizationSecurityKeyPublicKeyCredentialAssertion
```

## Overview

The security key creates an assertion when signing in with an existing credential. Use this class to verify the security key credential assertion when the authorization controller calls authorizationController(controller:didCompleteWithAuthorization:).

## Topics

### Instance Properties

var appID: Bool

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

class ASAuthorizationPlatformPublicKeyCredentialAssertion

A class that represents the platform credential assertion type.

protocol ASAuthorizationPublicKeyCredentialAssertionRequest

An interface for requesting a public key-based credential assertion.

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

