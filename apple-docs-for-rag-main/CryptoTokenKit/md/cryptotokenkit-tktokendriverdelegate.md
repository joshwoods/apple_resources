

- CryptoTokenKit
-  TKTokenDriverDelegate 

Protocol

# TKTokenDriverDelegate

The interface that a token driver delegate implements to respond to token creation events.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol TKTokenDriverDelegate : NSObjectProtocol
```

## Topics

### Creating and Removing Tokens

func tokenDriver(TKTokenDriver, terminateToken: TKToken)

Tells the delegate to terminate the token you specify.

func tokenDriver(TKTokenDriver, tokenFor: TKToken.Configuration) throws -> TKToken

Creates a new token for the configuration you specify.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- TKSmartCardTokenDriverDelegate

## See Also

### Responding to Token Creation

var delegate: (any TKTokenDriverDelegate)?

The token driver delegate.

typealias ClassID

The type of the class identifier for the token driver.

class Configuration

A configuration for one class of token.

