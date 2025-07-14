

- Authentication Services
- ASPasskeyCredentialRequestParameters
-  clientDataHash 

Instance Property

# clientDataHash

The client data that you sign as part of the response.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var clientDataHash: Data { get }
```

## See Also

### Viewing credential request parameters

var allowedCredentials: [Data]

A list of passkey credentials that the relying party accepts for this challenge.

var relyingPartyIdentifier: String

The relying party that issues the challenge.

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s preference for user verification.

