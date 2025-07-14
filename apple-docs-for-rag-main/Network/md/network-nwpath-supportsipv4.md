

- Network
- NWPath
-  supportsIPv4 

Instance Property

# supportsIPv4

A Boolean indicating whether the path can route IPv4 traffic.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
let supportsIPv4: Bool
```

## See Also

### Checking Path Capabilities

let supportsIPv6: Bool

A Boolean indicating whether the path can route IPv6 traffic.

let supportsDNS: Bool

A Boolean indicating whether the path has a DNS server configured.

var isConstrained: Bool

A Boolean indicating whether the path uses an interface in Low Data Mode.

let isExpensive: Bool

A Boolean indicating whether the path uses an interface that is considered expensive, such as Cellular or a Personal Hotspot.

