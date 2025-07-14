

- Network
- NWMulticastGroup
-  isUnicastDisabled 

Instance Property

# isUnicastDisabled

A Boolean that specifies whether the connection group rejects unicast traffic.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final let isUnicastDisabled: Bool
```

## See Also

### Inspecting Multicast Groups

var members: [NWEndpoint]

The set of IP multicast group addresses that the connection group joins.

let sourceFilter: NWEndpoint?

An optional address endpoint you provide to filter received multicast packets.

