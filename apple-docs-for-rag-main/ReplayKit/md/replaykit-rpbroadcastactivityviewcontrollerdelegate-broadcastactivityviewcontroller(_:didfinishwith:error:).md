

- ReplayKit
- RPBroadcastActivityViewControllerDelegate
-  broadcastActivityViewController(\_:didFinishWith:error:) 

Instance Method

# broadcastActivityViewController(\_:didFinishWith:error:)

Indicates that the broadcast activity view controller is ready to be dismissed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func broadcastActivityViewController(
    _ broadcastActivityViewController: RPBroadcastActivityViewController,
    didFinishWith broadcastController: RPBroadcastController?,
    error: (any Error)?
)
```

**Required**

## Parameters 

`broadcastActivityViewController`  

The broadcast activity view controller to be dismissed.

`broadcastController`  

Optional. The RPBroadcastController instance used to start and stop broadcasts to a selected service. When the user cancels service setup, this parameter is nil.

`error`  

An RPRecordingErrorDomain error. When a connection to a broadcast service has been set up successfully and the app is ready to broadcast, this parameter is `nil`.

## Discussion

When this method is called after a broadcast has been set up successfully, retain a reference to the RPBroadcastController instance contained in the `broadcastController` parameter to start and stop broadcasting.

