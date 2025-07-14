

- ReplayKit
- RPBroadcastActivityControllerDelegate
-  broadcastActivityController(\_:didFinishWith:error:) 

Instance Method

# broadcastActivityController(\_:didFinishWith:error:)

Tells the delegate that a user selected a broadcast.

macOS 11.0+

``` source
func broadcastActivityController(
    _ broadcastActivityController: RPBroadcastActivityController,
    didFinishWith broadcastController: RPBroadcastController?,
    error: (any Error)?
)
```

**Required**

## Parameters 

`broadcastActivityController`  

The broadcast activity controller instance.

`broadcastController`  

The broadcast controller instance used to start and stop broadcasts to a user selected service.

`error`  

An optional error indicating a failure.

