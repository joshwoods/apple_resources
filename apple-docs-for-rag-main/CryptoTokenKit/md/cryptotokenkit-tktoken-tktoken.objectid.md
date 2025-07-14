

- CryptoTokenKit
- TKToken
-  TKToken.ObjectID 

Type Alias

# TKToken.ObjectID

A unique and persistent identifier of a particular token object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
typealias ObjectID = Any
```

## Discussion

The type of this identifier must support property list serialization and must define its format by the implementation of the token extension.

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

class TKTokenKeychainKey

A token’s key as stored in the keychain.

