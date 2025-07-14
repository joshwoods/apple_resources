

- Authentication Services
- ASPasskeyCredentialRequest
-  supportedAlgorithms 

Instance Property

# supportedAlgorithms

A list of cryptographic signature algorithms that the relying party supports.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var supportedAlgorithms: [ASCOSEAlgorithmIdentifier] { get }
```

## Discussion

For credential assertion requests, this property is empty.

## See Also

### Viewing passkey challenge information

var clientDataHash: Data

The hash of the client data for this assertion.

var userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference

The relying party’s user verification preference.

