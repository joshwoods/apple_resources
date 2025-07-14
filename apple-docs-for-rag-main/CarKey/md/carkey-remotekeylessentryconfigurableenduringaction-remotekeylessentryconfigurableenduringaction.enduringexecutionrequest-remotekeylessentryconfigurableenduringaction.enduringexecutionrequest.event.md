

- CarKey
- RemoteKeylessEntryConfigurableEnduringAction
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest
-  RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event 

Enumeration

# RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event

iOS 18.0+iPadOS 18.0+macOS 15.0+watchOS 11.0+

``` source
enum Event
```

## Topics

### Enumeration Cases

case receivedContinuationRequest(RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.ContinuationRequest)

Received continuation request from the Vehicle executing the Enduring Action The enduring action may time out on the vehicle side if continuationRequest.continue() or stop() is not invoked promptly upon the receipt of this event.

