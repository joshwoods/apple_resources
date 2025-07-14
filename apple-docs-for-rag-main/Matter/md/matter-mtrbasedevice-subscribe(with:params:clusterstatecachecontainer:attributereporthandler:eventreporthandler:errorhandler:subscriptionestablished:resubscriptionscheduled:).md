

- Matter
- MTRBaseDevice
-  subscribe(with:params:clusterStateCacheContainer:attributeReportHandler:eventReportHandler:errorHandler:subscriptionEstablished:resubscriptionScheduled:) 

Instance Method

# subscribe(with:params:clusterStateCacheContainer:attributeReportHandler:eventReportHandler:errorHandler:subscriptionEstablished:resubscriptionScheduled:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func subscribe(
    with queue: dispatch_queue_t,
    params: MTRSubscribeParams,
    clusterStateCacheContainer: MTRClusterStateCacheContainer?,
    attributeReportHandler: MTRDeviceReportHandler?,
    eventReportHandler: MTRDeviceReportHandler?,
    errorHandler: @escaping MTRDeviceErrorHandler,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    resubscriptionScheduled: MTRDeviceResubscriptionScheduledHandler? = nil
)
```

