

- Security
-  SecKeySizes Deprecated

Enumeration

# SecKeySizes

The supported sizes for keys of various common types.

macOS 10.9–12.0Deprecated

``` source
enum SecKeySizes
```

Deprecated

No longer supported

## Topics

### Constants

case secDefaultKeySize

The default key size for the specified type.

case sec3DES192

192-bit DES.

case secAES128

128-bit AES.

static var secAES192: SecKeySizes

192-bit AES.

case secAES256

256-bit AES.

static var secp192r1: SecKeySizes

192-bit ECC Keys for Suite-B from RFC 4492 section 5.1.1.

static var secp256r1: SecKeySizes

256-bit ECC Keys for Suite-B from RFC 4492 section 5.1.1.

case secp384r1

384-bit ECC Keys for Suite-B from RFC 4492 section 5.1.1.

case secp521r1

521-bit ECC Keys for Suite-B from RFC 4492 section 5.1.1.

case secRSAMin

1024 bits is the minimum size for an RSA key.

case secRSAMax

4096 bits is the maximum size for an RSA key.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

