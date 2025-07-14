

- Matter
- MTRBaseClusterBasicInformation
-  subscribeAttributeProductAppearance(with:subscriptionEstablished:reportHandler:) 

Instance Method

# subscribeAttributeProductAppearance(with:subscriptionEstablished:reportHandler:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func subscribeAttributeProductAppearance(
    with params: MTRSubscribeParams,
    subscriptionEstablished: MTRSubscriptionEstablishedHandler?,
    reportHandler: @escaping (MTRBasicInformationClusterProductAppearanceStruct?, (any Error)?) -> Void
)
```

