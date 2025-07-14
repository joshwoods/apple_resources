

- CryptoTokenKit
-  TKToken 

Class

# TKToken

A representation of a hardware-based cryptographic token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKToken
```

## Overview

Note

When working with smart card tokens, use or inherit from the TKSmartCardToken subclass instead.

## Topics

### Creating Tokens

init(tokenDriver: TKTokenDriver, instanceID: TKToken.InstanceID)

Initializes a token with the driver you specify.

typealias InstanceID

A type that represents the instance identifier of a token.

### Responding to Session Creation

var delegate: (any TKTokenDelegate)?

The token delegate.

protocol TKTokenDelegate

The interface that a token delegate implements to respond to session creation events.

### Accessing the Driver

var tokenDriver: TKTokenDriver

The token driver.

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

typealias ObjectID

A unique and persistent identifier of a particular token object.

typealias ObjectID

A unique and persistent identifier of a particular token object.

### Configuring the Token

var configuration: TKToken.Configuration

The current configuration for a token.

class Configuration

A token’s configuration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKSmartCardToken

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Tokens

class TKTokenWatcher

An object that tracks the tokens available in the system.

class TKTokenDriver

A base class for building token drivers.

class TKTokenSession

A token session that manages the authentication state of a token.

