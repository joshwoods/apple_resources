

- Matter
- MTRClusterContentAppObserver
-  contentAppMessage(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# contentAppMessage(with:expectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func contentAppMessage(
    with params: MTRContentAppObserverClusterContentAppMessageParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRContentAppObserverClusterContentAppMessageResponseParams?, (any Error)?) -> Void
)
```

``` source
func contentAppMessage(
    with params: MTRContentAppObserverClusterContentAppMessageParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRContentAppObserverClusterContentAppMessageResponseParams
```

