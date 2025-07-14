

- Apple Archive
- ArchiveEncryptionContext
-  setSigningPrivateKey(\_:) 

Instance Method

# setSigningPrivateKey(\_:)

Sets the signing private key that corresponds to the signing public key that you used to create the archive.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func setSigningPrivateKey(_ key: P256.Signing.PrivateKey) throws
```

## Parameters 

`key`  

The signing private key.

## Discussion

If you set this on an encryption stream, you don’t need to set the corresponding public key because Apple Archive derives the public key from the private key.

If you only provide a signing public key to the encryption stream, sign the archive with a private key after closing the stream. Use a private key that corresponds to the signing public key that you used to create the archive.

## See Also

### Setting and retrieving keys

var mainKey: SymmetricKey?

The main key used to append data to an existing archive.

var symmetricKey: SymmetricKey?

The symmetric encryption key used to encrypt or decrypt an archive.

func generateSymmetricKey() throws -> SymmetricKey

Generates a symmetric encryption key.

func setSymmetricKey(SymmetricKey) throws

Sets the symmetric encryption key that the context requires for symmetric encryption mode.

func setRecipientPrivateKey(P256.KeyAgreement.PrivateKey) throws

Sets the recipient private key that the context requires to decrypt an archive to a specific recipient in ECDHE encryption profiles.

func setRecipientPublicKey(P256.KeyAgreement.PublicKey) throws

Sets the recipient public key that the context requires to encrypt an archive to a specific recipient in ECDHE encryption profiles.

func setSigningPublicKey(P256.Signing.PublicKey) throws

Sets the signing public key that the context requires to unlock a signed archive.

