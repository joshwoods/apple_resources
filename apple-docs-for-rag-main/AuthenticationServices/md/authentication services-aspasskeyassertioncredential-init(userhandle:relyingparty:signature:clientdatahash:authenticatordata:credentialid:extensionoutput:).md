

- Authentication Services
- ASPasskeyAssertionCredential
-  init(userHandle:relyingParty:signature:clientDataHash:authenticatorData:credentialID:extensionOutput:) 

Initializer

# init(userHandle:relyingParty:signature:clientDataHash:authenticatorData:credentialID:extensionOutput:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
convenience init(
    userHandle: Data,
    relyingParty: String,
    signature: Data,
    clientDataHash: Data,
    authenticatorData: Data,
    credentialID: Data,
    extensionOutput: ASPasskeyAssertionCredentialExtensionOutput?
)
```

