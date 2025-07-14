

- Matter
- MTRBaseDevice
-  subscribeAttribute(withEndpointId:clusterId:attributeId:minInterval:maxInterval:params:clientQueue:reportHandler:subscriptionEstablished:) Deprecated

Instance Method

# subscribeAttribute(withEndpointId:clusterId:attributeId:minInterval:maxInterval:params:clientQueue:reportHandler:subscriptionEstablished:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func subscribeAttribute(
    withEndpointId endpointId: NSNumber?,
    clusterId: NSNumber?,
    attributeId: NSNumber?,
    minInterval: NSNumber,
    maxInterval: NSNumber,
    params: MTRSubscribeParams?,
    clientQueue: dispatch_queue_t,
    reportHandler: @escaping MTRDeviceResponseHandler,
    subscriptionEstablished subscriptionEstablishedHandler: (() -> Void)? = nil
)
```

Deprecated

Please use subscribeToAttributesWithEndpointID:clusterID:attributeID:params:queue:reportHandler:subscriptionEstablished:

