

- Authentication Services
- ASAuthorizationPublicKeyCredentialAssertionRequest
-  userVerificationPreference 

Instance Property

# userVerificationPreference

A preference that indicates whether the authenticator attempts to verify the user at the time of sign-in.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference { get set }
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

var allowedCredentials: [any ASAuthorizationPublicKeyCredentialDescriptor]

A list of allowed credential descriptors the user attempts to sign in with.

**Required**

