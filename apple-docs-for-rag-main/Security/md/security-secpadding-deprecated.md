

- Security
-  SecPadding Deprecated

Structure

# SecPadding

The types of padding to use when you create or verify a digital signature.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.6–12.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
struct SecPadding
```

Deprecated

Replaced with SecKeyAlgorithm

## Topics

### Initializers

init(rawValue: UInt32)

### Constants

static var sigRaw: SecPadding

static var PKCS1: SecPadding

PKCS1 padding.

static var OAEP: SecPadding

static var PKCS1MD2: SecPadding

Data to be signed is an MD2 hash.

static var PKCS1MD5: SecPadding

Data to be signed is an MD5 hash.

static var PKCS1SHA1: SecPadding

Data to be signed is a SHA1 hash.

static var PKCS1SHA224: SecPadding

Data to be signed is a SHA224 hash.

static var PKCS1SHA256: SecPadding

Data to be signed is a SHA256 hash.

static var PKCS1SHA384: SecPadding

Data to be signed is a SHA384 hash.

static var PKCS1SHA512: SecPadding

Data to be signed is a SHA512 hash.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

