

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:getEstimatedSubscriptionLatencyWithReply:) 

Instance Method

# deviceController(\_:nodeID:getEstimatedSubscriptionLatencyWithReply:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    getEstimatedSubscriptionLatencyWithReply reply: @escaping (NSNumber?) -> Void
)
```

``` source
func deviceControllerGetEstimatedSubscriptionLatency(
    _ controller: UUID,
    nodeID: NSNumber
) async -> NSNumber?
```

**Required**

