

- CarKey
- RemoteKeylessEntryConfigurableEnduringAction
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event
-  RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event.receivedContinuationRequest(\_:) 

Case

# RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.Event.receivedContinuationRequest(\_:)

Received continuation request from the Vehicle executing the Enduring Action The enduring action may time out on the vehicle side if continuationRequest.continue() or stop() is not invoked promptly upon the receipt of this event.

iOS 18.0+iPadOS 18.0+macOS 15.0+watchOS 11.0+

``` source
case receivedContinuationRequest(RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.ContinuationRequest)
```

