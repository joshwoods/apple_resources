

- Matter
- MTRBaseDevice
-  subscribeToEvents(withEndpointID:clusterID:eventID:params:queue:reportHandler:subscriptionEstablished:) 

Instance Method

# subscribeToEvents(withEndpointID:clusterID:eventID:params:queue:reportHandler:subscriptionEstablished:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func subscribeToEvents(
    withEndpointID endpointID: NSNumber?,
    clusterID: NSNumber?,
    eventID: NSNumber?,
    params: MTRSubscribeParams?,
    queue: dispatch_queue_t,
    reportHandler: @escaping MTRDeviceResponseHandler,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler? = nil
)
```

