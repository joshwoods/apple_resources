

- Authentication Services
- ASAuthorizationPublicKeyCredentialRegistrationRequest
-  name 

Instance Property

# name

A user-visible name that identifies a credential.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var name: String { get set }
```

**Required**

## See Also

### Getting the properties

var attestationPreference: ASAuthorizationPublicKeyCredentialAttestationKind

The type of attestation you’re requesting.

**Required**

var challenge: Data

Arbitrary data that the client signs as proof of a valid registration or attestation.

**Required**

var displayName: String?

A user-visible name for the credential, such as the account’s user name.

**Required**

var relyingPartyIdentifier: String

The domain name of the website for the credential.

**Required**

var userID: Data

Data that the relying party associates with the credential.

**Required**

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

A preference for whether the authenticator attempts to verify the user at the time of sign-in.

**Required**

