

- CryptoTokenKit
-  TKTokenWatcher 

Class

# TKTokenWatcher

An object that tracks the tokens available in the system.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenWatcher
```

## Mentioned in 

Using Cryptographic Assets Stored on a Smart Card

## Overview

Create a token watcher and register an insertion handler to be notified when tokens are added to the system. You can also add removal handlers for specific tokens to be notified when those tokens are removed from the system.

## Topics

### Creating Token Watchers

init()

Initializes a token watcher.

init(insertionHandler: (String) -> Void)

Initializes a token watcher with the specified insertion handler.

Deprecated

### Accessing Token Identifiers

var tokenIDs: [String]

The token IDs currently available in the system.

### Configuring Handlers

func addRemovalHandler((String) -> Void, forTokenID: String)

Adds a removal handler for the specified token ID.

func setInsertionHandler((String) -> Void)

Sets an insertion handler closure to be called when a new token is inserted into the system.

### Classes

class TokenInfo

### Instance Methods

func tokenInfo(forTokenID: String) -> TKTokenWatcher.TokenInfo?

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

### Tokens

class TKTokenDriver

A base class for building token drivers.

class TKToken

A representation of a hardware-based cryptographic token.

class TKTokenSession

A token session that manages the authentication state of a token.

