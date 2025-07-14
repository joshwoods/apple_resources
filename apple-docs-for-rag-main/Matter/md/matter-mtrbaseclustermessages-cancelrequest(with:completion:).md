

- Matter
- MTRBaseClusterMessages
-  cancelRequest(with:completion:) 

Instance Method

# cancelRequest(with:completion:)

Command CancelMessagesRequest

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func cancelRequest(
    with params: MTRMessagesClusterCancelMessagesRequestParams,
    completion: @escaping MTRStatusCompletion
)
```

``` source
func cancelRequest(with params: MTRMessagesClusterCancelMessagesRequestParams) async throws
```

## Discussion

Command for cancelling message present requests

