

- Network
- NWProtocolIP
- NWProtocolIP.Metadata
-  ecn 

Instance Property

# ecn

A specific Explicit Congestion Notification flag value to set on an IP packet.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var ecn: NWProtocolIP.ECN { get set }
```

## See Also

### Sending IP Options

init()

Initializes an IP packet configuration with default settings.

enum ECN

Flag values for Explicit Congestion Notifications in IP packets.

var serviceClass: NWParameters.ServiceClass

A specific service class to mark on an IP packet.

