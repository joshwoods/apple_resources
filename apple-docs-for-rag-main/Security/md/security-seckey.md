

- Security
-  SecKey 

Class

# SecKey

An object that represents a cryptographic key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class SecKey
```

## Mentioned in 

Getting an Existing Key

## Overview

A SecKey instance that represents a key that is stored in a keychain can be safely cast to a SecKeychainItem for manipulation as a keychain item. On the other hand, if the key is not stored in a keychain, casting the object to a SecKeychainItem and passing it to Keychain Services functions returns errors.

## Relationships

### Conforms To

- Equatable
- Hashable

