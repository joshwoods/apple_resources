

- Matter
- MTRBaseDevice
-  subscribe(with:minInterval:maxInterval:params:cacheContainer:attributeReportHandler:eventReportHandler:errorHandler:subscriptionEstablished:resubscriptionScheduled:) Deprecated

Instance Method

# subscribe(with:minInterval:maxInterval:params:cacheContainer:attributeReportHandler:eventReportHandler:errorHandler:subscriptionEstablished:resubscriptionScheduled:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func subscribe(
    with queue: dispatch_queue_t,
    minInterval: UInt16,
    maxInterval: UInt16,
    params: MTRSubscribeParams?,
    cacheContainer attributeCacheContainer: MTRAttributeCacheContainer?,
    attributeReportHandler: MTRDeviceReportHandler?,
    eventReportHandler: MTRDeviceReportHandler?,
    errorHandler: @escaping MTRDeviceErrorHandler,
    subscriptionEstablished subscriptionEstablishedHandler: (() -> Void)?,
    resubscriptionScheduled resubscriptionScheduledHandler: MTRDeviceResubscriptionScheduledHandler? = nil
)
```

Deprecated

Please use subscribeWithQueue:params:clusterStateCacheContainer:attributeReportHandler:eventReportHandler:errorHandler:subscriptionEstablished:resubscriptionScheduled:

