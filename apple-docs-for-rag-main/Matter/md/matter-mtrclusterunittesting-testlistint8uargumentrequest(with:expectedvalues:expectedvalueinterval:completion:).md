

- Matter
- MTRClusterUnitTesting
-  testListInt8UArgumentRequest(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# testListInt8UArgumentRequest(with:expectedValues:expectedValueInterval:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func testListInt8UArgumentRequest(
    with params: MTRUnitTestingClusterTestListInt8UArgumentRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRUnitTestingClusterBooleanResponseParams?, (any Error)?) -> Void
)
```

``` source
func testListInt8UArgumentRequest(
    with params: MTRUnitTestingClusterTestListInt8UArgumentRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRUnitTestingClusterBooleanResponseParams
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testListInt8UArgumentRequest(with params: MTRUnitTestingClusterTestListInt8UArgumentRequestParams, expectedValues expectedDataValueDictionaries: [[String : Any]]?, expectedValueInterval expectedValueIntervalMs: NSNumber?) async throws -> MTRUnitTestingClusterBooleanResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

