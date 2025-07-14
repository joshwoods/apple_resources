

- CryptoTokenKit
- TKTokenDriver
- TKTokenDriver.Configuration
-  classID 

Instance Property

# classID

The class identifier of the token driver.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var classID: TKTokenDriver.ClassID { get }
```

## Discussion

The identifier uses a reverse-DNS format, such as `com.example.id`.

## See Also

### Reporting Configuration Information

var tokenConfigurations: [TKToken.InstanceID : TKToken.Configuration]

A dictionary of all currently configured tokens for this token class, which the token instance identifier keys.

class var driverConfigurations: [TKTokenDriver.ClassID : TKTokenDriver.Configuration]

A dictionary of token class configurations which the class identifier of the token driver keys.

