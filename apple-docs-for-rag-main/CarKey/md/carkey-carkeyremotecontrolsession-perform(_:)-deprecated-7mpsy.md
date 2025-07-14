

- CarKey
- CarKeyRemoteControlSession
-  perform(\_:) Deprecated

Instance Method

# perform(\_:)

Sends a request to the vehicle to start an action that has a separate stopping point.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.3–15.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func perform(_ enduringAction: RemoteKeylessEntryEnduringAction) throws -> RemoteKeylessEntryEnduringAction.EnduringExecutionRequest
```

Deprecated

Use perform(enduringAction:continuationStrategy:) instead

## Return Value

An object you use to get the results of the initial request and stop the action.

## Discussion

Call this method for vehicle features that that have both a start and stop point. For example, use it to start raising or lowering the top of a convertible. This method sends the request to the vehicle asynchronously.

Use the returned object to get the execution status of the initial request, and to optionally stop the action.

## See Also

### Performing Vehicle-Related Actions

func perform(RemoteKeylessEntryAction) throws -> RemoteKeylessEntryAction.ExecutionRequest

Sends a request to the vehicle to perform a one-time action.

