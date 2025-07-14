

- Authentication Services
- ASPasskeyCredentialRequestParameters
-  relyingPartyIdentifier 

Instance Property

# relyingPartyIdentifier

The relying party that issues the challenge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var relyingPartyIdentifier: String { get }
```

## See Also

### Viewing credential request parameters

var allowedCredentials: [Data]

A list of passkey credentials that the relying party accepts for this challenge.

var clientDataHash: Data

The client data that you sign as part of the response.

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s preference for user verification.

