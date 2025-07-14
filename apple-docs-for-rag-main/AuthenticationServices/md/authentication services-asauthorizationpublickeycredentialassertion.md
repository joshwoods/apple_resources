

- Authentication Services
-  ASAuthorizationPublicKeyCredentialAssertion 

Protocol

# ASAuthorizationPublicKeyCredentialAssertion

An interface for establishing a public key-based assertion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
protocol ASAuthorizationPublicKeyCredentialAssertion : ASPublicKeyCredential
```

## Overview

Both ASAuthorizationSecurityKeyPublicKeyCredentialAssertion and ASAuthorizationPlatformPublicKeyCredentialAssertion adhere to this interface.

## Topics

### Getting the properties

var signature: Data!

The signature for the assertion.

**Required**

var userID: Data!

A user identifier for the assertion.

**Required**

var rawAuthenticatorData: Data!

A byte sequence that contains additional information about the credential.

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

- ASAuthorizationPlatformPublicKeyCredentialAssertion
- ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

## See Also

### Account authentication

class ASAuthorizationPlatformPublicKeyCredentialAssertion

A class that represents the platform credential assertion type.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

A class that represents the security key credential assertion type.

protocol ASAuthorizationPublicKeyCredentialAssertionRequest

An interface for requesting a public key-based credential assertion.

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

