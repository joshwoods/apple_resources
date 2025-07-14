

- Apple Archive
- ArchiveEncryptionContext
-  setSigningPublicKey(\_:) 

Instance Method

# setSigningPublicKey(\_:)

Sets the signing public key that the context requires to unlock a signed archive.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func setSigningPublicKey(_ key: P256.Signing.PublicKey) throws
```

## Parameters 

`key`  

The recipient public key.

## Discussion

The public signing key is necessary to unlock a signed archive. If you don’t provide a private key when you create a new archive, provide a public key to tie the encryption to the signing identity. In this case, you need to sign the archive offline using the corresponding signing private key.

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

func setSigningPrivateKey(P256.Signing.PrivateKey) throws

Sets the signing private key that corresponds to the signing public key that you used to create the archive.

func setRecipientPublicKey(P256.KeyAgreement.PublicKey) throws

Sets the recipient public key that the context requires to encrypt an archive to a specific recipient in ECDHE encryption profiles.

