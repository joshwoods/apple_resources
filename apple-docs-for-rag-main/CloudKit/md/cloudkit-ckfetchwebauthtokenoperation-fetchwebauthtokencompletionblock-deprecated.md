

- CloudKit
- CKFetchWebAuthTokenOperation
-  fetchWebAuthTokenCompletionBlock Deprecated

Instance Property

# fetchWebAuthTokenCompletionBlock

The block to execute when the operation finishes.

iOS 9.2–15.0DeprecatediPadOS 9.2–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.11–12.0DeprecatedtvOS 9.1–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var fetchWebAuthTokenCompletionBlock: ((String?, (any Error)?) -> Void)? { get set }
```

Deprecated

Use fetchWebAuthTokenResultBlock instead

## Discussion

The closure returns no value and takes the following parameters:

- If the operation is successful, the web authentication token; otherwise, `nil`.

- An error that contains information about a problem, or `nil` if the system successfully fetches the token.

The operation executes this closure only once. Your closure must be capable of executing on a background thread, so any tasks that require access to the main thread must dispatch accordingly.

## See Also

### Managing the Operation’s Configuration

var apiToken: String?

The API token that allows access to an app’s container.

