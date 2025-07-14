

- Authentication Services
- ASPasskeyCredentialRequest
-  userVerificationPreference 

Instance Property

# userVerificationPreference

The relying party’s user verification preference.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference { get set }
```

## See Also

### Viewing passkey challenge information

var clientDataHash: Data

The hash of the client data for this assertion.

var supportedAlgorithms: [ASCOSEAlgorithmIdentifier]

A list of cryptographic signature algorithms that the relying party supports.

