

- CryptoTokenKit
-  TKTokenDriver 

Class

# TKTokenDriver

A base class for building token drivers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenDriver
```

## Overview

When using the TKTokenDriver class, implement the TKTokenDriverDelegate protocol with the tokenDriver(_:tokenFor:) method, which the system invokes when it requests the creation of a token instance. After you create the token driver, it can examine keychainItems and configurationData to implement your desired functionality.

An implementation can also access its associated token configuration using the TKToken.Configuration property.

Note

When working with smart card tokens, use or inherit from the TKSmartCardTokenDriver subclass instead.

## Topics

### Responding to Token Creation

var delegate: (any TKTokenDriverDelegate)?

The token driver delegate.

protocol TKTokenDriverDelegate

The interface that a token driver delegate implements to respond to token creation events.

typealias ClassID

The type of the class identifier for the token driver.

class Configuration

A configuration for one class of token.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKSmartCardTokenDriver

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

class TKToken

A representation of a hardware-based cryptographic token.

class TKTokenSession

A token session that manages the authentication state of a token.

