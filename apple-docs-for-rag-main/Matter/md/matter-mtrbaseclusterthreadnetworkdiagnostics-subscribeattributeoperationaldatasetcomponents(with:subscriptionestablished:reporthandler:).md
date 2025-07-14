

- Matter
- MTRBaseClusterThreadNetworkDiagnostics
-  subscribeAttributeOperationalDatasetComponents(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeOperationalDatasetComponents(with:subscriptionEstablished:reportHandler:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func subscribeAttributeOperationalDatasetComponents(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRThreadNetworkDiagnosticsClusterOperationalDatasetComponents?, (any Error)?) -> Void
)
```

