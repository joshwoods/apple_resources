

- Matter
- MTRClusterUnitTesting
-  testEmitTestEventRequest(with:expectedValues:expectedValueInterval:completion:) 

Instance Method

# testEmitTestEventRequest(with:expectedValues:expectedValueInterval:completion:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func testEmitTestEventRequest(
    with params: MTRUnitTestingClusterTestEmitTestEventRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completion: @escaping (MTRUnitTestingClusterTestEmitTestEventResponseParams?, (any Error)?) -> Void
)
```

``` source
func testEmitTestEventRequest(
    with params: MTRUnitTestingClusterTestEmitTestEventRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRUnitTestingClusterTestEmitTestEventResponseParams
```

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testEmitTestEventRequest(with params: MTRUnitTestingClusterTestEmitTestEventRequestParams, expectedValues expectedDataValueDictionaries: [[String : Any]]?, expectedValueInterval expectedValueIntervalMs: NSNumber?) async throws -> MTRUnitTestingClusterTestEmitTestEventResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

