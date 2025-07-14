

- Network
- NWProtocolTCP
- NWProtocolTCP.Options
-  keepaliveInterval 

Instance Property

# keepaliveInterval

The number of seconds that TCP waits between sending keepalive probes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var keepaliveInterval: Int { get set }
```

## See Also

### Configuring Keepalives

var enableKeepalive: Bool

A Boolean that enables TCP keepalives.

var keepaliveIdle: Int

The number of seconds of idleness that TCP waits before sending keepalive probes.

var keepaliveCount: Int

The number of keepalive probes that TCP sends before terminating the connection.

