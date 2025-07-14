

- CryptoTokenKit
-  TKTokenSession 

Class

# TKTokenSession

A token session that manages the authentication state of a token.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class TKTokenSession
```

## Overview

A token session communicates with its delegate to perform operations with its token that are bound to the authentication state.

A session is always instantiated by a TKToken instance through the token’s delegate when the framework detects access to the token from a new authentication session.

Important

Never share the authentication status of a token, such as the PIN entered to unlock a smart card, with other token sessions.

## Topics

### Creating Token Sessions

init(token: TKToken)

Initializes a token session with the specified token.

### Responding to Authentication Events

var delegate: (any TKTokenSessionDelegate)?

The token session delegate.

protocol TKTokenSessionDelegate

The interface that a session instance delegate implements to respond to token session authentication events.

### Accessing the Token

var token: TKToken

The token to which the session is bound.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKSmartCardTokenSession

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

class TKToken

A representation of a hardware-based cryptographic token.

