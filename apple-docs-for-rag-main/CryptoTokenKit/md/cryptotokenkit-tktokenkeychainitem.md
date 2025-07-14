

- CryptoTokenKit
-  TKTokenKeychainItem 

Class

# TKTokenKeychainItem

An abstract base class for managing a token’s contents as keychain items.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenKeychainItem
```

## Overview

Don’t use this base class directly. Instead, use one of its subclasses, such as TKTokenKeychainCertificate for managing certificates or TKTokenKeychainKey for managing cryptographic keys.

## Topics

### Creating Token Keychain Items

init(objectID: TKToken.ObjectID)

Initializes a token keychain item with the specified object ID.

### Accessing Keychain Item Attributes

var objectID: TKToken.ObjectID

Returns the object ID used for keychain item identification.

var label: String?

The user-visible label for the keychain item.

var constraints: [NSNumber : Any]?

Access constraints for the keychain item, keyed by TKTokenOperation values wrapped in NSNumber objects.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKTokenKeychainCertificate
- TKTokenKeychainKey

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

class TKTokenKeychainCertificate

A token’s certificate as stored in the keychain.

class TKTokenKeychainKey

A token’s key as stored in the keychain.

typealias ObjectID

A unique and persistent identifier of a particular token object.

typealias ObjectID

A unique and persistent identifier of a particular token object.

