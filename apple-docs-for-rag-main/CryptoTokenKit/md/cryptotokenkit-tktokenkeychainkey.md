

- CryptoTokenKit
-  TKTokenKeychainKey 

Class

# TKTokenKeychainKey

A token’s key as stored in the keychain.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeychainKey
```

## Topics

### Creating Token Keychain Keys

init?(certificate: SecCertificate?, objectID: TKToken.ObjectID)

Initializes a token keychain key with data from the specified certificate reference and a given object ID.

### Accessing Key Attributes

var keyType: String

The type of the key. Currently, only kSecAttrKeyTypeRSA and `kSecAttrKeyTypeECSECPrimeRandom` are supported values.

var keySizeInBits: Int

var applicationTag: Data?

The private tag data.

var publicKeyData: Data?

The public key data.

var publicKeyHash: Data?

The SHA1 hash of the raw public key.

var canDecrypt: Bool

Whether the key can be used to decrypt data.

var canSign: Bool

Whether the key can be used to sign data.

var canPerformKeyExchange: Bool

Whether the key can be used to perform Diffie-Hellman style cryptographic key exchange.

var isSuitableForLogin: Bool

Whether the key can be used for system login.

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

class TKTokenKeychainCertificate

A token’s certificate as stored in the keychain.

typealias ObjectID

A unique and persistent identifier of a particular token object.

typealias ObjectID

A unique and persistent identifier of a particular token object.

