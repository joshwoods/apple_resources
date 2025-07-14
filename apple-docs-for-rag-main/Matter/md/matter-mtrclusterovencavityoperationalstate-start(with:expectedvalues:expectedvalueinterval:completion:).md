

- Matter
- MTRClusterOvenCavityOperationalState
-  start(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# start(with:expectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func start(
    with params: MTROvenCavityOperationalStateClusterStartParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTROvenCavityOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void
)
```

``` source
func start(
    with params: MTROvenCavityOperationalStateClusterStartParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTROvenCavityOperationalStateClusterOperationalCommandResponseParams
```

