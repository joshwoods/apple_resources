

- Matter
- MTRBaseClusterContentAppObserver
-  contentAppMessage(with:completion:) 

Instance Method

# contentAppMessage(with:completion:)

Command ContentAppMessage

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func contentAppMessage(
    with params: MTRContentAppObserverClusterContentAppMessageParams,
    completion: @escaping (MTRContentAppObserverClusterContentAppMessageResponseParams?, (any Error)?) -> Void
)
```

``` source
func contentAppMessage(with params: MTRContentAppObserverClusterContentAppMessageParams) async throws -> MTRContentAppObserverClusterContentAppMessageResponseParams
```

## Discussion

Upon receipt, the data field MAY be parsed and interpreted. Message encoding is specific to the Content App. A Content App MAY when possible read attributes from the Basic Information Cluster on the Observer and use this to determine the Message encoding.

