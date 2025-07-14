

- Matter
- MTRClusterChannel
-  getProgramGuide(withExpectedValues:expectedValueInterval:completion:) 

Instance Method

# getProgramGuide(withExpectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getProgramGuide(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRChannelClusterProgramGuideResponseParams?, (any Error)?) -> Void
)
```

``` source
func programGuide(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRChannelClusterProgramGuideResponseParams
```

