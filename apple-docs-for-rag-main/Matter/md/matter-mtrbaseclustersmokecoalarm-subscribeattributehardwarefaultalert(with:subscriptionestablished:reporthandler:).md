

- Matter
- MTRBaseClusterSmokeCOAlarm
-  subscribeAttributeHardwareFaultAlert(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeHardwareFaultAlert(with:subscriptionEstablished:reportHandler:)

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
func subscribeAttributeHardwareFaultAlert(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (NSNumber?, (any Error)?) -> Void
)
```

