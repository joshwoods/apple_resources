

- Apple Archive
- ArchiveEncryptionContext
-  mainKey 

Instance Property

# mainKey

The main key used to append data to an existing archive.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var mainKey: SymmetricKey? { get set }
```

## Discussion

Use the main key to append data to an existing AEA archive with the encryptionStream(appendingTo:encryptionContext:flags:threadCount:) function.

You can use the original credentials for symmetric key or password encryption. You need this key to reopen archives created with the ECDHE profiles.

The main key can’t be used to open the stream for decryption.

## See Also

### Setting and retrieving keys

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

func setSigningPublicKey(P256.Signing.PublicKey) throws

Sets the signing public key that the context requires to unlock a signed archive.

