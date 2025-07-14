

- Security
- Security Transforms
-  Transform Attributes 

API Collection

# Transform Attributes

Specify the attributes of a transform.

## Overview

Use these keys and values when accessing transform attributes by name, such as with the SecTransformSetAttribute(_:_:_:_:) and SecTransformGetAttribute(_:_:) functions. You can also use some of the values directly in certain function calls, such as when you create a encode transform with the SecEncodeTransformCreate(_:_:) function and give it an `encodeType` parameter to seed the kSecEncodeTypeAttribute attribute.

## Topics

### Encode and Decode Keys

let kSecEncodeLineLengthAttribute: CFString

The length of encoded Base32 or Base64 lines.

Deprecated

let kSecEncodeTypeAttribute: CFString

The encoding used by an encode transform.

Deprecated

let kSecDecodeTypeAttribute: CFString

The encoding used by a decode transform.

let kSecCompressionRatio: CFString

The compression ratio.

Deprecated

### Digest and Encryption Keys

let kSecDigestTypeAttribute: CFString

The digest algorithm.

Deprecated

let kSecDigestLengthAttribute: CFString

The digest length.

Deprecated

let kSecDigestHMACKeyAttribute: CFString

The key for HMAC operation.

Deprecated

let kSecInputIsAttributeName: CFString

The type of input to the transform.

Deprecated

let kSecEncryptionMode: CFString

The encryption mode.

Deprecated

let kSecEncryptKey: CFString

The encryption key for the transform.

Deprecated

let kSecIVKey: CFString

The setting for an initialization vector.

Deprecated

let kSecPaddingKey: CFString

The kind of padding to use.

Deprecated

let kSecOAEPEncodingParametersAttributeName: CFString

The OAEP encoding parameters.

Deprecated

let kSecOAEPMGF1DigestAlgorithmAttributeName: CFString

The OAEP MGF1 digest algorithm.

Deprecated

let kSecOAEPMessageLengthAttributeName: CFString

The OAEP message length.

Deprecated

### Transform Keys

let kSecTransformInputAttributeName: CFString

The input to a transform.

Deprecated

let kSecTransformOutputAttributeName: CFString

The output of a transform.

Deprecated

let kSecTransformDebugAttributeName: CFString

A write stream that should receive debug data.

Deprecated

let kSecKeyAttributeName: CFString

The cryptographic key associated with a transform.

let kSecSignatureAttributeName: CFString

The cryptographic signature associated with a transform.

let kSecTransformAbortAttributeName: CFString

The reason for an abort.

Deprecated

let kSecTransformTransformName: CFString

The name of a transform.

Deprecated

### Encode Types

Values you use with the kSecEncodeTypeAttribute and kSecDecodeTypeAttribute keys.

let kSecBase32Encoding: CFString

A base 32 encoding.

Deprecated

let kSecBase64Encoding: CFString

A base 64 encoding.

Deprecated

let kSecZLibEncoding: CFString

A compressed encoding.

Deprecated

### Digest Types

Values you use with the kSecDigestTypeAttribute key.

let kSecDigestMD2: CFString

An MD2 digest.

Deprecated

let kSecDigestMD4: CFString

An MD4 digest.

Deprecated

let kSecDigestMD5: CFString

An MD5 digest.

Deprecated

let kSecDigestSHA1: CFString

An SHA1 digest.

Deprecated

let kSecDigestSHA2: CFString

An SHA2 digest.

Deprecated

let kSecDigestHMACMD5: CFString

An HMAC using the MD5 digest algorithm.

Deprecated

let kSecDigestHMACSHA1: CFString

An HMAC using the SHA1 digest algorithm.

Deprecated

let kSecDigestHMACSHA2: CFString

An HMAC using one of the SHA2 digest algorithms.

Deprecated

### Line Lengths

Values you use with the kSecEncodeLineLengthAttribute key.

let kSecLineLength64: CFString

A line length of 64 bytes.

Deprecated

let kSecLineLength76: CFString

A line length of 76 bytes.

Deprecated

### Input Types

Values you use with the kSecInputIsAttributeName key.

let kSecInputIsDigest: CFString

The input is a digest of the original data.

let kSecInputIsPlainText: CFString

The input is plain text.

let kSecInputIsRaw: CFString

The input is raw.

Deprecated

### Padding Types

Values you use with the kSecPaddingKey key.

let kSecPaddingNoneKey: CFString

No padding will be used when encrypting or decrypting.

Deprecated

let kSecPaddingOAEPKey: CFString

PKCS7 padding will be used when encrypting or decrypting.

Deprecated

let kSecPaddingPKCS1Key: CFString

PKCS1 padding will be used when encrypting or decrypting.

Deprecated

let kSecPaddingPKCS5Key: CFString

PKCS5 padding will be used when encrypting or decrypting.

Deprecated

let kSecPaddingPKCS7Key: CFString

PKCS7 padding will be used when encrypting or decrypting.

Deprecated

### Encryption Modes

Values you use with the kSecEncryptionMode key.

let kSecModeNoneKey: CFString

No mode will be used when encrypting or decrypting.

Deprecated

let kSecModeCBCKey: CFString

CBC mode will be used when encrypting or decrypting.

Deprecated

let kSecModeCFBKey: CFString

CFB mode will be used when encrypting or decrypting.

Deprecated

let kSecModeECBKey: CFString

ECB mode will be used when encrypting or decrypting.

Deprecated

let kSecModeOFBKey: CFString

OFB mode will be used when encrypting or decrypting.

Deprecated

