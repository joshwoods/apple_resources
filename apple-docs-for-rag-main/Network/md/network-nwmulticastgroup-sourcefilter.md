

- Network
- NWMulticastGroup
-  sourceFilter 

Instance Property

# sourceFilter

An optional address endpoint you provide to filter received multicast packets.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final let sourceFilter: NWEndpoint?
```

## See Also

### Inspecting Multicast Groups

var members: [NWEndpoint]

The set of IP multicast group addresses that the connection group joins.

let isUnicastDisabled: Bool

A Boolean that specifies whether the connection group rejects unicast traffic.

