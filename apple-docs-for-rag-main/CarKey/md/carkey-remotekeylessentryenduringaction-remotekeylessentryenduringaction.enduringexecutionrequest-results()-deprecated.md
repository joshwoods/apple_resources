

- CarKey
- RemoteKeylessEntryEnduringAction
- RemoteKeylessEntryEnduringAction.EnduringExecutionRequest
-  results() Deprecated

Instance Method

# results()

Returns the results of a preceding action request.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
final func results() async throws -> ExecutionStatus
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Return Value

A structure that contains the vehicle-specific status code from the vehicle.

## Discussion

After you call your session’s perform(_:) method to send an action request to a vehicle, call this method to await the results of that request. Upon the successful completion of the request, this method returns the vehicle-provided status code. If an error occurs, this method throws the error instead.

## See Also

### Getting the Vehicle’s Respose

struct ExecutionStatus

A type that contains the status code a vehicle returns after executing an action.

