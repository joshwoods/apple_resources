

- CryptoTokenKit
-  TKTokenKeychainCertificate 

Class

# TKTokenKeychainCertificate

A token’s certificate as stored in the keychain.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeychainCertificate
```

## Topics

### Creating Token Keychain Certificates

init?(certificate: SecCertificate, objectID: TKToken.ObjectID)

Initializes a token keychain certificate with data from the specified certificate reference and a given object ID.

### Accessing Certificate Data

var data: Data

Returns a DER-encoded representation of an X.509 certificate.

## Relationships

### Inherits From

- TKTokenKeychainItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Accessing Keychain Items

var keychainContents: TKTokenKeychainContents?

The contents of the keychain for this token.

class TKTokenKeychainContents

A representation of the state of the keychain for a particular token.

class TKTokenKeychainItem

An abstract base class for managing a token’s contents as keychain items.

class TKTokenKeychainKey

A token’s key as stored in the keychain.

typealias ObjectID

A unique and persistent identifier of a particular token object.

typealias ObjectID

A unique and persistent identifier of a particular token object.

