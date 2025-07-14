

- Authentication Services
- ASPasskeyCredentialRequestParameters
-  userVerificationPreference 

Instance Property

# userVerificationPreference

The relying party’s preference for user verification.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference { get }
```

## See Also

### Viewing credential request parameters

var allowedCredentials: [Data]

A list of passkey credentials that the relying party accepts for this challenge.

var clientDataHash: Data

The client data that you sign as part of the response.

var relyingPartyIdentifier: String

The relying party that issues the challenge.

