

- Authentication Services
- ASPasskeyCredentialRequest
-  init(credentialIdentity:clientDataHash:userVerificationPreference:supportedAlgorithms:extensionInput:) 

Initializer

# init(credentialIdentity:clientDataHash:userVerificationPreference:supportedAlgorithms:extensionInput:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
convenience init(
    credentialIdentity: ASPasskeyCredentialIdentity,
    clientDataHash: Data,
    userVerificationPreference: ASAuthorizationPublicKeyCredentialUserVerificationPreference,
    supportedAlgorithms: [ASCOSEAlgorithmIdentifier],
    extensionInput: ASPasskeyAssertionCredentialExtensionInput?
)
```

