

- CarKey
- RemoteKeylessEntryConfigurableEnduringAction
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest
-  stop() 

Instance Method

# stop()

Sends a request to stop a previously started action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
final func stop() throws
```

## Discussion

This method sends the cancellation request asynchronously to the vehicle. If you call the results method again, the method delivers the results of the cancellation request.

