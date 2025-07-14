

- Matter
- MTRBaseClusterTestCluster
-  subscribeAttributeNullableStruct(withMinInterval:maxInterval:params:subscriptionEstablished:reportHandler:) Deprecated

Instance Method

# subscribeAttributeNullableStruct(withMinInterval:maxInterval:params:subscriptionEstablished:reportHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func subscribeAttributeNullableStruct(
    withMinInterval minInterval: NSNumber,
    maxInterval: NSNumber,
    params: MTRSubscribeParams?,
    subscriptionEstablished subscriptionEstablishedHandler: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRTestClusterClusterSimpleStruct?, (any Error)?) -> Void
)
```

Deprecated

Please use subscribeAttributeNullableStructWithParams:subscriptionEstablished:

