

- CryptoTokenKit
-  TKTokenKeychainContents 

Class

# TKTokenKeychainContents

A representation of the state of the keychain for a particular token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeychainContents
```

## Topics

### Adding Keychain Items

func fill(with: [TKTokenKeychainItem])

Fills the keychain with the specified items.

### Accessing Keychain Items

var items: [TKTokenKeychainItem]

Returns all items for token in the keychain.

func key(forObjectID: TKToken.ObjectID) throws -> TKTokenKeychainKey

Returns the key for a specified object identifier.

func certificate(forObjectID: TKToken.ObjectID) throws -> TKTokenKeychainCertificate

Returns the key for a specified object identifier.

## Relationships

### Inherits From

- NSObject

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

class TKTokenKeychainItem

An abstract base class for managing a token’s contents as keychain items.

class TKTokenKeychainCertificate

A token’s certificate as stored in the keychain.

class TKTokenKeychainKey

A token’s key as stored in the keychain.

typealias ObjectID

A unique and persistent identifier of a particular token object.

typealias ObjectID

A unique and persistent identifier of a particular token object.

