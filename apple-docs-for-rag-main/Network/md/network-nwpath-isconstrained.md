

- Network
- NWPath
-  isConstrained 

Instance Property

# isConstrained

A Boolean indicating whether the path uses an interface in Low Data Mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var isConstrained: Bool { get }
```

## See Also

### Checking Path Capabilities

let supportsIPv4: Bool

A Boolean indicating whether the path can route IPv4 traffic.

let supportsIPv6: Bool

A Boolean indicating whether the path can route IPv6 traffic.

let supportsDNS: Bool

A Boolean indicating whether the path has a DNS server configured.

let isExpensive: Bool

A Boolean indicating whether the path uses an interface that is considered expensive, such as Cellular or a Personal Hotspot.

