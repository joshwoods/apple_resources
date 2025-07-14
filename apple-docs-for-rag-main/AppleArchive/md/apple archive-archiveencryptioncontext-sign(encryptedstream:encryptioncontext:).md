

- Apple Archive
- ArchiveEncryptionContext
-  sign(encryptedStream:encryptionContext:) 

Type Method

# sign(encryptedStream:encryptionContext:)

Signs an encrypted archive using the credentials stored in the specified encryption context.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func sign(
    encryptedStream: ArchiveByteStream,
    encryptionContext context: ArchiveEncryptionContext
) throws
```

## Parameters 

`encryptedStream`  

A read-write byte stream that points to an encrypted archive.

`context`  

The encryption context that provides the credentials.

## Discussion

Close the encrypted stream before calling this function, and create the archive with a `signatureMode` other than none. Create the context that you pass to this function from the same archive and it must contain the signature encryption key and the signing private key.

## See Also

### Signing an encryption context

var signatureMode: ArchiveEncryptionContext.SignatureMode

The signature mode, such as an ECDSA Nist P-256 signature.

struct SignatureMode

Constants that describe the signature modes of an encryption context.

