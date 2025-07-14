

- Matter
- MTRClusterOTASoftwareUpdateProvider
-  applyUpdateRequest(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# applyUpdateRequest(with:expectedValues:expectedValueInterval:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func applyUpdateRequest(
    with params: MTROTASoftwareUpdateProviderClusterApplyUpdateRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTROTASoftwareUpdateProviderClusterApplyUpdateResponseParams?, (any Error)?) -> Void
)
```

``` source
func applyUpdateRequest(
    with params: MTROTASoftwareUpdateProviderClusterApplyUpdateRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTROTASoftwareUpdateProviderClusterApplyUpdateResponseParams
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func applyUpdateRequest(with params: MTROTASoftwareUpdateProviderClusterApplyUpdateRequestParams, expectedValues expectedDataValueDictionaries: [[String : Any]]?, expectedValueInterval expectedValueIntervalMs: NSNumber?) async throws -> MTROTASoftwareUpdateProviderClusterApplyUpdateResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

