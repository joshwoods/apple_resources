

- Matter
- MTRClusterEnergyEVSE
-  getTargetsWithExpectedValues(\_:expectedValueInterval:completion:) 

Instance Method

# getTargetsWithExpectedValues(\_:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getTargetsWithExpectedValues(
    _ expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTREnergyEVSEClusterGetTargetsResponseParams?, (any Error)?) -> Void
)
```

``` source
func targets(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTREnergyEVSEClusterGetTargetsResponseParams
```

