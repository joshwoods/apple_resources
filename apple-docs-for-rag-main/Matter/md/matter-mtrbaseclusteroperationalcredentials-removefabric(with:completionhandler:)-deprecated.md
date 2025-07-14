

- Matter
- MTRBaseClusterOperationalCredentials
-  removeFabric(with:completionHandler:) Deprecated

Instance Method

# removeFabric(with:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func removeFabric(
    with params: MTROperationalCredentialsClusterRemoveFabricParams,
    completionHandler: @escaping (MTROperationalCredentialsClusterNOCResponseParams?, (any Error)?) -> Void
)
```

``` source
func removeFabric(with params: MTROperationalCredentialsClusterRemoveFabricParams) async throws -> MTROperationalCredentialsClusterNOCResponseParams
```

Deprecated

Please use removeFabricWithParams:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func removeFabric(with params: MTROperationalCredentialsClusterRemoveFabricParams) async throws -> MTROperationalCredentialsClusterNOCResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

