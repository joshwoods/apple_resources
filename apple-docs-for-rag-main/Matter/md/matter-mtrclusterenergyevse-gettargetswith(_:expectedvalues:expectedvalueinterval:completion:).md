

- Matter
- MTRClusterEnergyEVSE
-  getTargetsWith(\_:expectedValues:expectedValueInterval:completion:) 

Instance Method

# getTargetsWith(\_:expectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func getTargetsWith(
    _ params: MTREnergyEVSEClusterGetTargetsParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTREnergyEVSEClusterGetTargetsResponseParams?, (any Error)?) -> Void
)
```

``` source
func targets(
    with params: MTREnergyEVSEClusterGetTargetsParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTREnergyEVSEClusterGetTargetsResponseParams
```

