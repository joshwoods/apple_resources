

- Matter
- MTRBaseClusterTestCluster
-  testListNestedStructListArgumentRequest(with:completionHandler:) Deprecated

Instance Method

# testListNestedStructListArgumentRequest(with:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func testListNestedStructListArgumentRequest(
    with params: MTRTestClusterClusterTestListNestedStructListArgumentRequestParams,
    completionHandler: @escaping (MTRTestClusterClusterBooleanResponseParams?, (any Error)?) -> Void
)
```

``` source
func testListNestedStructListArgumentRequest(with params: MTRTestClusterClusterTestListNestedStructListArgumentRequestParams) async throws -> MTRTestClusterClusterBooleanResponseParams
```

Deprecated

Please use testListNestedStructListArgumentRequestWithParams:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testListNestedStructListArgumentRequest(with params: MTRTestClusterClusterTestListNestedStructListArgumentRequestParams) async throws -> MTRTestClusterClusterBooleanResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

