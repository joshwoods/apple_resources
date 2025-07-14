

- Security
-  SecKeyAlgorithm 

Structure

# SecKeyAlgorithm

The algorithms that cryptographic keys enable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct SecKeyAlgorithm
```

## Topics

### Elliptic curve encryption standard X963

static let eciesEncryptionStandardX963SHA1AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardX963SHA224AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardX963SHA256AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardX963SHA384AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardX963SHA512AESGCM: SecKeyAlgorithm

### Elliptic curve encryption standard variable IVX963

static let eciesEncryptionStandardVariableIVX963SHA224AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardVariableIVX963SHA256AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardVariableIVX963SHA384AESGCM: SecKeyAlgorithm

static let eciesEncryptionStandardVariableIVX963SHA512AESGCM: SecKeyAlgorithm

### Elliptic curve encryption cofactor variable IVX963

static let eciesEncryptionCofactorVariableIVX963SHA224AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorVariableIVX963SHA256AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorVariableIVX963SHA384AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorVariableIVX963SHA512AESGCM: SecKeyAlgorithm

### Elliptic curve encryption cofactor X963

static let eciesEncryptionCofactorX963SHA1AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorX963SHA224AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorX963SHA256AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorX963SHA384AESGCM: SecKeyAlgorithm

static let eciesEncryptionCofactorX963SHA512AESGCM: SecKeyAlgorithm

### Elliptic curve signature RFC4754

static let ecdsaSignatureRFC4754: SecKeyAlgorithmDeprecated

### Elliptic curve signature digest RFC4754

static let ecdsaSignatureDigestRFC4754: SecKeyAlgorithm

An algorithm for generating message digest signatures.

static let ecdsaSignatureDigestRFC4754SHA1: SecKeyAlgorithm

An algorithm for generating signatures of SHA1 message digests.

static let ecdsaSignatureDigestRFC4754SHA224: SecKeyAlgorithm

An algorithm for generating signatures of SHA224 message digests.

static let ecdsaSignatureDigestRFC4754SHA256: SecKeyAlgorithm

An algorithm for generating signatures of SHA256 message digests.

static let ecdsaSignatureDigestRFC4754SHA384: SecKeyAlgorithm

An algorithm for generating signatures of SHA384 message digests.

static let ecdsaSignatureDigestRFC4754SHA512: SecKeyAlgorithm

An algorithm for generating signatures of SHA512 message digests.

### Elliptic curve signature message RFC4754

static let ecdsaSignatureMessageRFC4754SHA1: SecKeyAlgorithm

An algorithm for generating message signatures by calculating and signing the SHA1 message digest.

static let ecdsaSignatureMessageRFC4754SHA224: SecKeyAlgorithm

An algorithm for generating message signatures by calculating and signing the SHA224 message digest.

static let ecdsaSignatureMessageRFC4754SHA256: SecKeyAlgorithm

An algorithm for generating message signatures by calculating and signing the SHA256 message digest.

static let ecdsaSignatureMessageRFC4754SHA384: SecKeyAlgorithm

An algorithm for generating message signatures by calculating and signing the SHA384 message digest.

static let ecdsaSignatureMessageRFC4754SHA512: SecKeyAlgorithm

An algorithm for generating message signatures by calculating and signing the SHA512 message digest.

### Elliptic curve signature digest X962

static let ecdsaSignatureDigestX962: SecKeyAlgorithm

static let ecdsaSignatureDigestX962SHA1: SecKeyAlgorithm

static let ecdsaSignatureDigestX962SHA224: SecKeyAlgorithm

static let ecdsaSignatureDigestX962SHA256: SecKeyAlgorithm

static let ecdsaSignatureDigestX962SHA384: SecKeyAlgorithm

static let ecdsaSignatureDigestX962SHA512: SecKeyAlgorithm

### Elliptic curve signature message X962

static let ecdsaSignatureMessageX962SHA1: SecKeyAlgorithm

static let ecdsaSignatureMessageX962SHA224: SecKeyAlgorithm

static let ecdsaSignatureMessageX962SHA256: SecKeyAlgorithm

static let ecdsaSignatureMessageX962SHA384: SecKeyAlgorithm

static let ecdsaSignatureMessageX962SHA512: SecKeyAlgorithm

### Elliptic curve key exchange

static let ecdhKeyExchangeCofactor: SecKeyAlgorithm

static let ecdhKeyExchangeStandard: SecKeyAlgorithm

static let ecdhKeyExchangeCofactorX963SHA1: SecKeyAlgorithm

static let ecdhKeyExchangeStandardX963SHA1: SecKeyAlgorithm

static let ecdhKeyExchangeCofactorX963SHA224: SecKeyAlgorithm

static let ecdhKeyExchangeCofactorX963SHA256: SecKeyAlgorithm

static let ecdhKeyExchangeCofactorX963SHA384: SecKeyAlgorithm

static let ecdhKeyExchangeCofactorX963SHA512: SecKeyAlgorithm

static let ecdhKeyExchangeStandardX963SHA224: SecKeyAlgorithm

static let ecdhKeyExchangeStandardX963SHA256: SecKeyAlgorithm

static let ecdhKeyExchangeStandardX963SHA384: SecKeyAlgorithm

static let ecdhKeyExchangeStandardX963SHA512: SecKeyAlgorithm

### RSA encryption

static let rsaEncryptionRaw: SecKeyAlgorithm

static let rsaEncryptionPKCS1: SecKeyAlgorithm

### RSA encryption OAEP

static let rsaEncryptionOAEPSHA1: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA224: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA256: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA384: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA512: SecKeyAlgorithm

### RSA encryption OAEP AESGCM

static let rsaEncryptionOAEPSHA1AESGCM: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA224AESGCM: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA256AESGCM: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA384AESGCM: SecKeyAlgorithm

static let rsaEncryptionOAEPSHA512AESGCM: SecKeyAlgorithm

### RSA signature raw

static let rsaSignatureRaw: SecKeyAlgorithm

### RSA signature digest PKCS1v15

static let rsaSignatureDigestPKCS1v15Raw: SecKeyAlgorithm

static let rsaSignatureDigestPKCS1v15SHA1: SecKeyAlgorithm

static let rsaSignatureDigestPKCS1v15SHA224: SecKeyAlgorithm

static let rsaSignatureDigestPKCS1v15SHA256: SecKeyAlgorithm

static let rsaSignatureDigestPKCS1v15SHA384: SecKeyAlgorithm

static let rsaSignatureDigestPKCS1v15SHA512: SecKeyAlgorithm

### RSA signature message PKCS1v15

static let rsaSignatureMessagePKCS1v15SHA1: SecKeyAlgorithm

static let rsaSignatureMessagePKCS1v15SHA224: SecKeyAlgorithm

static let rsaSignatureMessagePKCS1v15SHA256: SecKeyAlgorithm

static let rsaSignatureMessagePKCS1v15SHA384: SecKeyAlgorithm

static let rsaSignatureMessagePKCS1v15SHA512: SecKeyAlgorithm

### RSA signature digest PSS

static let rsaSignatureDigestPSSSHA1: SecKeyAlgorithm

static let rsaSignatureDigestPSSSHA224: SecKeyAlgorithm

static let rsaSignatureDigestPSSSHA256: SecKeyAlgorithm

static let rsaSignatureDigestPSSSHA384: SecKeyAlgorithm

static let rsaSignatureDigestPSSSHA512: SecKeyAlgorithm

### RSA signature message PSS

static let rsaSignatureMessagePSSSHA1: SecKeyAlgorithm

static let rsaSignatureMessagePSSSHA224: SecKeyAlgorithm

static let rsaSignatureMessagePSSSHA256: SecKeyAlgorithm

static let rsaSignatureMessagePSSSHA384: SecKeyAlgorithm

static let rsaSignatureMessagePSSSHA512: SecKeyAlgorithm

### Initializers

init(rawValue: CFString)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

