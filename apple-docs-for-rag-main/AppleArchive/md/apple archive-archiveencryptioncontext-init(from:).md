

- Apple Archive
- ArchiveEncryptionContext
-  init(from:) 

Initializer

# init(from:)

Returns a new encryption context from the specified encrypted stream.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init?(from stream: ArchiveByteStream)
```

## Parameters 

`stream`  

The encrypted stream that provides the profile, signature mode, encryption mode, and authorization data.

## Discussion

Use this function to either reopen an encrypted stream for writing or open an encrypted stream for reading. After you open the encryption context, query the archive properties and insert the credentials necessary to unlock and sign the stream.

In the case of a signed stream, if you’ve set a private signing key with AEAContextSetSigningPrivateKey the context signs the stream on close.

If you haven’t set a private key, the context still requires a public key, as it’s tied to the stream. After you close the encryption stream, you can pass the private signing key to the context by calling the stream-signing function AEAStreamSign.

## See Also

### Creating an archive encryption context

init(profile: ArchiveEncryptionContext.Profile, compressionAlgorithm: ArchiveCompression, compressionBlockSize: Int)

Returns a new encryption context from the specified profile, compression algorithm, and block size.

