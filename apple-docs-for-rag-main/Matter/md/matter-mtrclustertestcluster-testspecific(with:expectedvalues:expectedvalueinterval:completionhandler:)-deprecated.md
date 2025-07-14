

- Matter
- MTRClusterTestCluster
-  testSpecific(with:expectedValues:expectedValueInterval:completionHandler:) Deprecated

Instance Method

# testSpecific(with:expectedValues:expectedValueInterval:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func testSpecific(
    with params: MTRTestClusterClusterTestSpecificParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?,
    completionHandler: @escaping (MTRTestClusterClusterTestSpecificResponseParams?, (any Error)?) -> Void
)
```

``` source
func testSpecific(
    with params: MTRTestClusterClusterTestSpecificParams?,
    expectedValues expectedDataValueDictionaries: [[String : Any]]?,
    expectedValueInterval expectedValueIntervalMs: NSNumber?
) async throws -> MTRTestClusterClusterTestSpecificResponseParams
```

Deprecated

Please use testSpecificWithParams:expectedValues:expectedValueInterval:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func testSpecific(with params: MTRTestClusterClusterTestSpecificParams?, expectedValues expectedDataValueDictionaries: [[String : Any]]?, expectedValueInterval expectedValueIntervalMs: NSNumber?) async throws -> MTRTestClusterClusterTestSpecificResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

