

- CarKey
- RemoteKeylessEntryEnduringAction
- RemoteKeylessEntryEnduringAction.EnduringExecutionRequest
-  stop() Deprecated

Instance Method

# stop()

Sends a request to stop a previously started action.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
final func stop() throws
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Discussion

This method sends the cancellation request asynchronously to the vehicle. If you call the results method again, the method delivers the results of the cancellation request.

