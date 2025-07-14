

- Apple Archive
- ArchiveEncryptionContext
- ArchiveEncryptionContext.Profile
-  hkdf_sha256_aesctr_hmac\_\_symmetric\_\_none 

Type Property

# hkdf_sha256_aesctr_hmac\_\_symmetric\_\_none

A constant that represents unsigned, symmetric key encryption.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static let hkdf_sha256_aesctr_hmac__symmetric__none: ArchiveEncryptionContext.Profile
```

## See Also

### Profile Constants

static let hkdf_sha256_hmac__none__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents no encryption, authenticated container, signature is mandatory.

static let hkdf_sha256_aesctr_hmac__symmetric__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents signed symmetric key encryption, signed with encrypted signature.

static let hkdf_sha256_aesctr_hmac__ecdhe_p256__none: ArchiveEncryptionContext.Profile

A constant that represents unsigned ECDHE public key encryption, where only the recipient with the corresponding private key can unlock the container.

static let hkdf_sha256_aesctr_hmac__ecdhe_p256__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents signed ECDHE public key encryption, where only the recipient with the corresponding private key can unlock the container.

static let hkdf_sha256_aesctr_hmac__scrypt__none: ArchiveEncryptionContext.Profile

A constant that represents unsigned password encryption using scrypt.

