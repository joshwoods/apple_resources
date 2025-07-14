

- Network
- NWProtocolTCP
- NWProtocolTCP.Options
-  persistTimeout 

Instance Property

# persistTimeout

The TCP persist timeout, in seconds, as defined by RFC 6429.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var persistTimeout: Int { get set }
```

## See Also

### Setting Timeouts

var connectionTimeout: Int

The number of seconds that TCP waits before timing out its handshake.

var connectionDropTime: Int

The timeout, in seconds, for TCP retransmission attempts.

