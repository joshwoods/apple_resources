

- Matter
- MTRBaseClusterTimeSynchronization
-  subscribeAttributeUTCTime(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeUTCTime(with:subscriptionEstablished:reportHandler:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func subscribeAttributeUTCTime(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (NSNumber?, (any Error)?) -> Void
)
```

