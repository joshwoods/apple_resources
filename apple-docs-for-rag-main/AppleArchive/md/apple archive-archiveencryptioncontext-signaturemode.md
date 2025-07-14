

- Apple Archive
- ArchiveEncryptionContext
-  signatureMode 

Instance Property

# signatureMode

The signature mode, such as an ECDSA Nist P-256 signature.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var signatureMode: ArchiveEncryptionContext.SignatureMode { get }
```

## See Also

### Signing an encryption context

static func sign(encryptedStream: ArchiveByteStream, encryptionContext: ArchiveEncryptionContext) throws

Signs an encrypted archive using the credentials stored in the specified encryption context.

struct SignatureMode

Constants that describe the signature modes of an encryption context.

