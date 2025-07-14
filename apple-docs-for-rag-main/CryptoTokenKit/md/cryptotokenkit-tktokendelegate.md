

- CryptoTokenKit
-  TKTokenDelegate 

Protocol

# TKTokenDelegate

The interface that a token delegate implements to respond to session creation events.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol TKTokenDelegate : NSObjectProtocol
```

## Topics

### Delegate Methods

func createSession(TKToken) throws -> TKTokenSession

Tells the delegate to create a session for the specified token.

**Required**

func token(TKToken, terminateSession: TKTokenSession)

Tells the delegate to terminate the specified token session.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to Session Creation

var delegate: (any TKTokenDelegate)?

The token delegate.

