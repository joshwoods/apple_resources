

- Matter
- MTRBaseClusterTestCluster
-  subscribeAttributeWriteOnlyInt8u(withMinInterval:maxInterval:params:subscriptionEstablished:reportHandler:) Deprecated

Instance Method

# subscribeAttributeWriteOnlyInt8u(withMinInterval:maxInterval:params:subscriptionEstablished:reportHandler:)

iOS 16.2–16.4DeprecatediPadOS 16.2–16.4DeprecatedMac Catalyst 16.2–16.4DeprecatedmacOS 13.1–13.3DeprecatedtvOS 16.2–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.2–9.4Deprecated

``` source
func subscribeAttributeWriteOnlyInt8u(
    withMinInterval minInterval: NSNumber,
    maxInterval: NSNumber,
    params: MTRSubscribeParams?,
    subscriptionEstablished subscriptionEstablishedHandler: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (NSNumber?, (any Error)?) -> Void
)
```

Deprecated

Please use subscribeAttributeWriteOnlyInt8uWithParams:subscriptionEstablished:

