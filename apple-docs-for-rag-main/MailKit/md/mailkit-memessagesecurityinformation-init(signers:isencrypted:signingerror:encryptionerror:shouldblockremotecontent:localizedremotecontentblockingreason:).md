

- MailKit
- MEMessageSecurityInformation
-  init(signers:isEncrypted:signingError:encryptionError:shouldBlockRemoteContent:localizedRemoteContentBlockingReason:) 

Initializer

# init(signers:isEncrypted:signingError:encryptionError:shouldBlockRemoteContent:localizedRemoteContentBlockingReason:)

macOS 12.0+

``` source
init(
    signers: [MEMessageSigner],
    isEncrypted: Bool,
    signingError: (any Error)?,
    encryptionError: (any Error)?,
    shouldBlockRemoteContent: Bool,
    localizedRemoteContentBlockingReason: String?
)
```

