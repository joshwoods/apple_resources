

- Matter
- MTRClusterChannel
-  getProgramGuide(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# getProgramGuide(with:expectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getProgramGuide(
    with params: MTRChannelClusterGetProgramGuideParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void
)
```

``` source
func programGuide(
    with params: MTRChannelClusterGetProgramGuideParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRChannelClusterProgramGuideResponseParams
```

