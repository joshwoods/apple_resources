

- Authentication Services
- ASAuthorizationPublicKeyCredentialAssertionRequest
-  allowedCredentials 

Instance Property

# allowedCredentials

A list of allowed credential descriptors the user attempts to sign in with.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var allowedCredentials: [any ASAuthorizationPublicKeyCredentialDescriptor] { get set }
```

**Required**

## See Also

### Getting the properties

var challenge: Data

The challenge to sign.

**Required**

var relyingPartyIdentifier: String

The domain name of the website for the credential.

**Required**

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

A preference that indicates whether the authenticator attempts to verify the user at the time of sign-in.

**Required**

