

- CarKey
- RemoteKeylessEntryAction
- RemoteKeylessEntryAction.ExecutionRequest
-  results() 

Instance Method

# results()

Returns the results of a preceding action request.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
final func results() async throws -> ExecutionStatus
```

## Return Value

A structure that contains the vehicle-specific status code from the vehicle.

## Discussion

After you call your session’s perform(_:) method to send an action request to a vehicle, call this method and await the results of that request. Upon the successful completion of the request, this method returns the vehicle-provided status code. If an error occurs, this method throws the error instead.

## See Also

### Getting the Vehicle’s Respose

struct ExecutionStatus

A type that contains the status code a vehicle returns after executing an action.

