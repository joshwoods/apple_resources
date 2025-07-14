

- Matter
- MTRBaseClusterRVCOperationalState
-  subscribeAttributeOperationalError(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeOperationalError(with:subscriptionEstablished:reportHandler:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
func subscribeAttributeOperationalError(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRRVCOperationalStateClusterErrorStateStruct?, (any Error)?) -> Void
)
```

