

- CryptoTokenKit
- TKTokenDriver
-  TKTokenDriver.Configuration 

Class

# TKTokenDriver.Configuration

A configuration for one class of token.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class Configuration
```

## Topics

### Reporting Configuration Information

var classID: TKTokenDriver.ClassID

The class identifier of the token driver.

var tokenConfigurations: [TKToken.InstanceID : TKToken.Configuration]

A dictionary of all currently configured tokens for this token class, which the token instance identifier keys.

class var driverConfigurations: [TKTokenDriver.ClassID : TKTokenDriver.Configuration]

A dictionary of token class configurations which the class identifier of the token driver keys.

### Adding and Removing Configurations

func addTokenConfiguration(for: TKToken.InstanceID) -> TKToken.Configuration

Creates a configuration object for a token with the token instance identifier you specify.

func removeTokenConfiguration(for: TKToken.InstanceID)

Removes a configuration for a token with the token instance identifier you specify.

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

### Responding to Token Creation

var delegate: (any TKTokenDriverDelegate)?

The token driver delegate.

protocol TKTokenDriverDelegate

The interface that a token driver delegate implements to respond to token creation events.

typealias ClassID

The type of the class identifier for the token driver.

