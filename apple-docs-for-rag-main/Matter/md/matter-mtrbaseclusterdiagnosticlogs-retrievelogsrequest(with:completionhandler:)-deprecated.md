

- Matter
- MTRBaseClusterDiagnosticLogs
-  retrieveLogsRequest(with:completionHandler:) Deprecated

Instance Method

# retrieveLogsRequest(with:completionHandler:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
func retrieveLogsRequest(
    with params: MTRDiagnosticLogsClusterRetrieveLogsRequestParams,
    completionHandler: @escaping (MTRDiagnosticLogsClusterRetrieveLogsResponseParams?, (any Error)?) -> Void
)
```

``` source
func retrieveLogsRequest(with params: MTRDiagnosticLogsClusterRetrieveLogsRequestParams) async throws -> MTRDiagnosticLogsClusterRetrieveLogsResponseParams
```

Deprecated

Please use retrieveLogsRequestWithParams:completion:

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func retrieveLogsRequest(with params: MTRDiagnosticLogsClusterRetrieveLogsRequestParams) async throws -> MTRDiagnosticLogsClusterRetrieveLogsResponseParams
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

