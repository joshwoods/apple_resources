

- Matter
- MTRBaseDevice
-  subscribe(toAttributePaths:eventPaths:params:queue:reportHandler:subscriptionEstablished:resubscriptionScheduled:) 

Instance Method

# subscribe(toAttributePaths:eventPaths:params:queue:reportHandler:subscriptionEstablished:resubscriptionScheduled:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func subscribe(
    toAttributePaths attributePaths: [MTRAttributeRequestPath]?,
    eventPaths: [MTREventRequestPath]?,
    params: MTRSubscribeParams?,
    queue: dispatch_queue_t,
    reportHandler: @escaping MTRDeviceResponseHandler,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    resubscriptionScheduled: MTRDeviceResubscriptionScheduledHandler? = nil
)
```

