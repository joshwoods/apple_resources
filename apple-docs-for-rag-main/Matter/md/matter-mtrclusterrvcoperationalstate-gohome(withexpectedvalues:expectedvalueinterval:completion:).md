

- Matter
- MTRClusterRVCOperationalState
-  goHome(withExpectedValues:expectedValueInterval:completion:) 

Instance Method

# goHome(withExpectedValues:expectedValueInterval:completion:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func goHome(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRRVCOperationalStateClusterOperationalCommandResponseParams?, (any Error)?) -> Void
)
```

``` source
func goHome(
    withExpectedValues expectedValues: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRRVCOperationalStateClusterOperationalCommandResponseParams
```

