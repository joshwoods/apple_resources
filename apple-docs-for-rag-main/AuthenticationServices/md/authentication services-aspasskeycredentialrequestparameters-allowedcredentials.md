

- Authentication Services
- ASPasskeyCredentialRequestParameters
-  allowedCredentials 

Instance Property

# allowedCredentials

A list of passkey credentials that the relying party accepts for this challenge.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var allowedCredentials: [Data] { get }
```

## Discussion

If the array is empty, then the relying party accepts any passkey credential.

## See Also

### Viewing credential request parameters

var clientDataHash: Data

The client data that you sign as part of the response.

var relyingPartyIdentifier: String

The relying party that issues the challenge.

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s preference for user verification.

