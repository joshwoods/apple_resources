

- Authentication Services
-  ASAuthorizationCredential 

Protocol

# ASAuthorizationCredential

An interface that all credentials share.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ASAuthorizationCredential : NSCopying, NSSecureCoding, NSObjectProtocol
```

## Relationships

### Inherits From

- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Inherited By

- ASAuthorizationPublicKeyCredentialAssertion
- ASAuthorizationPublicKeyCredentialRegistration
- ASPublicKeyCredential

### Conforming Types

- ASAuthorizationAppleIDCredential
- ASAuthorizationPlatformPublicKeyCredentialAssertion
- ASAuthorizationPlatformPublicKeyCredentialRegistration
- ASAuthorizationSecurityKeyPublicKeyCredentialAssertion
- ASAuthorizationSecurityKeyPublicKeyCredentialRegistration
- ASAuthorizationSingleSignOnCredential
- ASOneTimeCodeCredential
- ASPasskeyAssertionCredential
- ASPasskeyRegistrationCredential
- ASPasswordCredential

## See Also

### Getting the Credential

var credential: any ASAuthorizationCredential

Information provided about a user after successful authentication.

