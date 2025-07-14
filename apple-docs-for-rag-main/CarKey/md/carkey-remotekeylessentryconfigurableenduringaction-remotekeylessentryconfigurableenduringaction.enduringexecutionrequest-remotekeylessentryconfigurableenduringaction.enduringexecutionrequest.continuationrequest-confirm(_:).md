

- CarKey
- RemoteKeylessEntryConfigurableEnduringAction
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest
- RemoteKeylessEntryConfigurableEnduringAction.EnduringExecutionRequest.ContinuationRequest
-  confirm(\_:) 

Instance Method

# confirm(\_:)

Method for your app to acknowledge receipt of this continuation request and commit to continue execution of this enduring action with optional arbitrary data to send to the vehicle. There is a maximum length of 64 bytes for the data to be sent.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func confirm(_ data: Data? = nil) throws
```

