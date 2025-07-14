

- ARKit
- ARSessionObserver
-  sessionWasInterrupted(\_:) 

Instance Method

# sessionWasInterrupted(\_:)

Tells the delegate that the session has temporarily stopped processing frames and tracking device position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func sessionWasInterrupted(_ session: ARSession)
```

## Parameters 

`session`  

The session providing information.

## Discussion

A session is interrupted when it fails to receive camera or motion sensing data. Session interruptions occur whenever camera capture is not available—for example, when your app is in the background or there are multiple foreground apps—or when the device is too busy to process motion sensor data.

Important

An interruption is equivalent to manually pausing the session. Do not call pause() in response to this callback, as that prevents your app from being notified when the interruption ends.

## See Also

### Handling Interruptions

func sessionInterruptionEnded(ARSession)

Tells the delegate that the session has resumed processing frames and tracking device position.

func sessionShouldAttemptRelocalization(ARSession) -> Bool

Asks the delegate whether to attempt recovery of world-tracking state after an interruption.

