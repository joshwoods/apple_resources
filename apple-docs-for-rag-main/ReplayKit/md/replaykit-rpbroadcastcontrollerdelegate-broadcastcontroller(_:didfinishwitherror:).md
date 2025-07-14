

- ReplayKit
- RPBroadcastControllerDelegate
-  broadcastController(\_:didFinishWithError:) 

Instance Method

# broadcastController(\_:didFinishWithError:)

Tells the delegate that a broadcast ended due to an error.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
optional func broadcastController(
    _ broadcastController: RPBroadcastController,
    didFinishWithError error: (any Error)?
)
```

**Required**

## Parameters 

`broadcastController`  

The current controller instance.

`error`  

An RPRecordingErrorCode error indicating why the broadcast finished.

## Discussion

Use the returned error to inform the user why the broadcast failed and provide an option to resume the broadcast, if applicable.

