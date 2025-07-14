

- Security
-  tls_ciphersuite_t 

Enumeration

# tls_ciphersuite_t

The collection of valid ciphersuites.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum tls_ciphersuite_t
```

## Topics

### AES

case AES_128_GCM_SHA256

case AES_256_GCM_SHA384

### Cha Cha Poly

case CHACHA20_POLY1305_SHA256

### Elliptic Curve

case ECDHE_ECDSA_WITH_3DES_EDE_CBC_SHADeprecated

case ECDHE_ECDSA_WITH_AES_128_CBC_SHA

case ECDHE_ECDSA_WITH_AES_128_CBC_SHA256

case ECDHE_ECDSA_WITH_AES_128_GCM_SHA256

case ECDHE_ECDSA_WITH_AES_256_CBC_SHA

case ECDHE_ECDSA_WITH_AES_256_CBC_SHA384

case ECDHE_ECDSA_WITH_AES_256_GCM_SHA384

case ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256

case ECDHE_RSA_WITH_3DES_EDE_CBC_SHADeprecated

case ECDHE_RSA_WITH_AES_128_CBC_SHA

case ECDHE_RSA_WITH_AES_128_CBC_SHA256

case ECDHE_RSA_WITH_AES_128_GCM_SHA256

case ECDHE_RSA_WITH_AES_256_CBC_SHA

case ECDHE_RSA_WITH_AES_256_CBC_SHA384

case ECDHE_RSA_WITH_AES_256_GCM_SHA384

case ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256

### RSA

case RSA_WITH_3DES_EDE_CBC_SHADeprecated

case RSA_WITH_AES_128_CBC_SHA

case RSA_WITH_AES_128_CBC_SHA256

case RSA_WITH_AES_128_GCM_SHA256

case RSA_WITH_AES_256_CBC_SHA

case RSA_WITH_AES_256_CBC_SHA256

case RSA_WITH_AES_256_GCM_SHA384

### Initializers

init?(rawValue: UInt16)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

