

- Matter
- MTRClusterOvenMode
-  changeToMode(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# changeToMode(with:expectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func changeToMode(
    with params: MTROvenModeClusterChangeToModeParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTROvenModeClusterChangeToModeResponseParams?, (any Error)?) -> Void
)
```

``` source
func changeToMode(
    with params: MTROvenModeClusterChangeToModeParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTROvenModeClusterChangeToModeResponseParams
```

