

- Network
- NWMulticastGroup
-  members 

Instance Property

# members

The set of IP multicast group addresses that the connection group joins.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var members: [NWEndpoint] { get }
```

## See Also

### Inspecting Multicast Groups

let sourceFilter: NWEndpoint?

An optional address endpoint you provide to filter received multicast packets.

let isUnicastDisabled: Bool

A Boolean that specifies whether the connection group rejects unicast traffic.

