

- Network
- NWProtocolUDP
- NWProtocolUDP.Options
-  preferNoChecksum 

Instance Property

# preferNoChecksum

A Boolean that configures the connection to not send UDP checksums.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var preferNoChecksum: Bool { get set }
```

## Discussion

UDP checksums are optional when the datagrams are sent over IPv4. This option configures UDP to not set checksums on these datagrams, but has no effect on IPv6.

## See Also

### Customizing UDP Connections

init()

Initializes a default set of UDP connection options.

