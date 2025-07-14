

- CryptoTokenKit
- TKTokenDriver
- TKTokenDriver.Configuration
-  tokenConfigurations 

Instance Property

# tokenConfigurations

A dictionary of all currently configured tokens for this token class, which the token instance identifier keys.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var tokenConfigurations: [TKToken.InstanceID : TKToken.Configuration] { get }
```

## See Also

### Reporting Configuration Information

var classID: TKTokenDriver.ClassID

The class identifier of the token driver.

class var driverConfigurations: [TKTokenDriver.ClassID : TKTokenDriver.Configuration]

A dictionary of token class configurations which the class identifier of the token driver keys.

