

- Authentication Services
- ASAuthorizationPublicKeyCredentialAssertionRequest
-  relyingPartyIdentifier 

Instance Property

# relyingPartyIdentifier

The domain name of the website for the credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var relyingPartyIdentifier: String { get set }
```

**Required**

## See Also

### Getting the properties

var challenge: Data

The challenge to sign.

**Required**

var allowedCredentials: [any ASAuthorizationPublicKeyCredentialDescriptor]

A list of allowed credential descriptors the user attempts to sign in with.

**Required**

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

A preference that indicates whether the authenticator attempts to verify the user at the time of sign-in.

**Required**

