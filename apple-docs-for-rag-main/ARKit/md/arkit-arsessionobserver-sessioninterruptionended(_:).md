

- ARKit
- ARSessionObserver
-  sessionInterruptionEnded(\_:) 

Instance Method

# sessionInterruptionEnded(\_:)

Tells the delegate that the session has resumed processing frames and tracking device position.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func sessionInterruptionEnded(_ session: ARSession)
```

## Parameters 

`session`  

The session providing information.

## Discussion

After a session has been interrupted (see the sessionWasInterrupted(_:) delegate method), it automatically resumes running whenever the conditions that caused the interruption improve.

When a session resumes, it continues tracking from its last known state. However, if the device has moved since the interruption began, the ARKit world coordinate system and anchor positions no longer match their original real-world frame of reference. To attempt recovery of world tracking from before the interruption, implement the sessionShouldAttemptRelocalization(_:) delegate method.

## See Also

### Handling Interruptions

func sessionWasInterrupted(ARSession)

Tells the delegate that the session has temporarily stopped processing frames and tracking device position.

func sessionShouldAttemptRelocalization(ARSession) -> Bool

Asks the delegate whether to attempt recovery of world-tracking state after an interruption.

