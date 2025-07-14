

- CryptoTokenKit
- TKTokenDriver
- TKTokenDriver.Configuration
-  driverConfigurations 

Type Property

# driverConfigurations

A dictionary of token class configurations which the class identifier of the token driver keys.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class var driverConfigurations: [TKTokenDriver.ClassID : TKTokenDriver.Configuration] { get }
```

## Discussion

If the app hosting the token extension calls this method, it returns a list of configurations for hosted token extensions. Otherwise, this method returns an empty array.

## See Also

### Reporting Configuration Information

var classID: TKTokenDriver.ClassID

The class identifier of the token driver.

var tokenConfigurations: [TKToken.InstanceID : TKToken.Configuration]

A dictionary of all currently configured tokens for this token class, which the token instance identifier keys.

