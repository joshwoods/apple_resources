

- Network
- IPAddress
-  isLoopback 

Instance Property

# isLoopback

A Boolean indicating whether this address is a loopback address for the local device.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var isLoopback: Bool { get }
```

**Required**

## See Also

### Inspecting Address Properties

var rawValue: Data

The raw data of an IP address.

**Required**

var interface: NWInterface?

The interface associated with this address, such as the IPv6 scoped interface.

**Required**

var isLinkLocal: Bool

A Boolean indicating whether this address is in a link-local range.

**Required**

var isMulticast: Bool

A Boolean indicating whether this address is a multicast address.

**Required**

