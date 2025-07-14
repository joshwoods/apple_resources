

- Matter
- MTRBaseClusterMessages
-  presentRequest(with:completion:) 

Instance Method

# presentRequest(with:completion:)

Command PresentMessagesRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func presentRequest(
    with params: MTRMessagesClusterPresentMessagesRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func presentRequest(with params: MTRMessagesClusterPresentMessagesRequestParams) async throws
```

## Discussion

Command for requesting messages be presented

