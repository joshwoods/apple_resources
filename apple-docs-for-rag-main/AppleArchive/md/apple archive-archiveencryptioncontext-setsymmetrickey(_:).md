

- Apple Archive
- ArchiveEncryptionContext
-  setSymmetricKey(\_:) 

Instance Method

# setSymmetricKey(\_:)

Sets the symmetric encryption key that the context requires for symmetric encryption mode.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func setSymmetricKey(_ key: SymmetricKey) throws
```

## Parameters 

`key`  

The symmetric encryption key.

## Discussion

Use this function to set the encryption key for a context with a symmetric profile.

## See Also

### Related Documentation

struct SymmetricKey

A symmetric cryptographic key.

### Setting and retrieving keys

var mainKey: SymmetricKey?

The main key used to append data to an existing archive.

var symmetricKey: SymmetricKey?

The symmetric encryption key used to encrypt or decrypt an archive.

func generateSymmetricKey() throws -> SymmetricKey

Generates a symmetric encryption key.

func setRecipientPrivateKey(P256.KeyAgreement.PrivateKey) throws

Sets the recipient private key that the context requires to decrypt an archive to a specific recipient in ECDHE encryption profiles.

func setSigningPrivateKey(P256.Signing.PrivateKey) throws

Sets the signing private key that corresponds to the signing public key that you used to create the archive.

func setRecipientPublicKey(P256.KeyAgreement.PublicKey) throws

Sets the recipient public key that the context requires to encrypt an archive to a specific recipient in ECDHE encryption profiles.

func setSigningPublicKey(P256.Signing.PublicKey) throws

Sets the signing public key that the context requires to unlock a signed archive.

