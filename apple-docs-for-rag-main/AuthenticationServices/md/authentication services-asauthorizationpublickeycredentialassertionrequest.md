

- Authentication Services
-  ASAuthorizationPublicKeyCredentialAssertionRequest 

Protocol

# ASAuthorizationPublicKeyCredentialAssertionRequest

An interface for requesting a public key-based credential assertion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
protocol ASAuthorizationPublicKeyCredentialAssertionRequest : NSCopying, NSSecureCoding, NSObjectProtocol
```

## Topics

### Getting the properties

var challenge: Data

The challenge to sign.

**Required**

var relyingPartyIdentifier: String

The domain name of the website for the credential.

**Required**

var allowedCredentials: [any ASAuthorizationPublicKeyCredentialDescriptor]

A list of allowed credential descriptors the user attempts to sign in with.

**Required**

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

A preference that indicates whether the authenticator attempts to verify the user at the time of sign-in.

**Required**

## Relationships

### Inherits From

- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialAssertionRequest
- ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

## See Also

### Account authentication

protocol ASAuthorizationPublicKeyCredentialAssertion

An interface for establishing a public key-based assertion.

class ASAuthorizationPlatformPublicKeyCredentialAssertion

A class that represents the platform credential assertion type.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertion

A class that represents the security key credential assertion type.

class ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

The concrete assertion request type for platform credentials.

class ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

A class that defines the assertion request type for security key credentials.

