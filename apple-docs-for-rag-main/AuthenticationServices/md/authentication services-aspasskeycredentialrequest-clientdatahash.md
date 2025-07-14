

- Authentication Services
- ASPasskeyCredentialRequest
-  clientDataHash 

Instance Property

# clientDataHash

The hash of the client data for this assertion.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var clientDataHash: Data { get }
```

## Discussion

Use the client data hash for both registration and assertion challenges.

## See Also

### Viewing passkey challenge information

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s user verification preference.

var supportedAlgorithms: [ASCOSEAlgorithmIdentifier]

A list of cryptographic signature algorithms that the relying party supports.

