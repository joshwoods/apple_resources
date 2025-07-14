

- Network
- IPv6Address
-  multicastScope 

Instance Property

# multicastScope

The IPv6 multicast scope of the address.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var multicastScope: IPv6Address.Scope? { get }
```

## See Also

### Inspecting Address Properties

var rawValue: Data

The raw data of an IPv6 address.

let interface: NWInterface?

The IPv6 scoped interface associated with this address.

enum Scope

An IPv6 multicast scope.

var isAny: Bool

A Boolean indicating whether the address is the unspecified address (::).

var is6to4: Bool

A Boolean indicating whether the address is a 6to4 address.

var isIPv4Compatabile: Bool

A Boolean indicating whether the address is IPv4-compatible.

var isIPv4Mapped: Bool

A Boolean indicating whether the address is an IPv4-mapped address.

var isLinkLocal: Bool

A Boolean indicating whether this address is in a link-local range.

var isLoopback: Bool

A Boolean indicating whether this address is a loopback address for the local device.

var isMulticast: Bool

A Boolean indicating whether this address is a multicast address.

