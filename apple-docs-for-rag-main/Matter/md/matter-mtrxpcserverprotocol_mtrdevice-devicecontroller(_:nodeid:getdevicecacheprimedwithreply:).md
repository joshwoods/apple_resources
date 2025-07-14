

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:getDeviceCachePrimedWithReply:) 

Instance Method

# deviceController(\_:nodeID:getDeviceCachePrimedWithReply:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    getDeviceCachePrimedWithReply reply: @escaping (Bool) -> Void
)
```

``` source
func deviceControllerGetDeviceCachePrimed(
    _ controller: UUID,
    nodeID: NSNumber
) async -> Bool
```

**Required**

