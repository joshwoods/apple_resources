

- Matter
- MTRClusterTestCluster
-  testListInt8UArgumentRequest(with:expectedValues:expectedValueInterval:completionHandler:) Deprecated

Instance Method

# testListInt8UArgumentRequest(with:expectedValues:expectedValueInterval:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func testListInt8UArgumentRequest(
    with params: MTRTestClusterClusterTestListInt8UArgumentRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completionHandler: @escaping (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void
)
```

``` source
func testListInt8UArgumentRequest(
    with params: MTRTestClusterClusterTestListInt8UArgumentRequestParams,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRTestClusterClusterBooleanResponseParams
```

Deprecated

Please use testListInt8UArgumentRequestWithParams:expectedValues:expectedValueInterval:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testListInt8UArgumentRequest(with params: MTRTestClusterClusterTestListInt8UArgumentRequestParams, expectedValues expectedDataValueDictionaries: [[String : Any]]?, expectedValueInterval expectedValueIntervalMs: NSNumber?) async throws -> MTRTestClusterClusterBooleanResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

