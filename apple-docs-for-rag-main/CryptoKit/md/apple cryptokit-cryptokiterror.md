

- Apple CryptoKit
-  CryptoKitError 

Enumeration

# CryptoKitError

General cryptography errors used by CryptoKit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CryptoKitError
```

## Topics

### Reporting errors

case incorrectKeySize

The key size is incorrect.

case invalidParameter

The parameter is invalid.

case incorrectParameterSize

The parameter size is incorrect.

case underlyingCoreCryptoError(error: Int32)

The underlying corecrypto library is unable to complete the requested action.

case authenticationFailure

The authentication tag or signature is incorrect.

case wrapFailure

The framework can’t wrap the specified key.

case unwrapFailure

The framework can’t unwrap the specified key.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum CryptoKitASN1Error

Errors from decoding ASN.1 content.

