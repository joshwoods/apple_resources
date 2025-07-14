

- CryptoTokenKit
- TKToken
- TKToken.Configuration
-  instanceID 

Instance Property

# instanceID

The unique, persistent identifier of this token that the token implementation creates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var instanceID: TKToken.InstanceID { get }
```

## Discussion

The instance identifier often represents some kind of serial number of the target hardware.

## See Also

### Reporting Configuration Information

var configurationData: Data?

Additional configuration information for the token instance.

