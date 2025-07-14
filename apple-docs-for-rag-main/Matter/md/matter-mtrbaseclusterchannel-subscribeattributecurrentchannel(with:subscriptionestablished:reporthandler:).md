

- Matter
- MTRBaseClusterChannel
-  subscribeAttributeCurrentChannel(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeCurrentChannel(with:subscriptionEstablished:reportHandler:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func subscribeAttributeCurrentChannel(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRChannelClusterChannelInfoStruct?, (any Error)?) -> Void
)
```

