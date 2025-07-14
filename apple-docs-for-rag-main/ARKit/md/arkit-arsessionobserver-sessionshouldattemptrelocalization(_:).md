

- ARKit
- ARSessionObserver
-  sessionShouldAttemptRelocalization(\_:) 

Instance Method

# sessionShouldAttemptRelocalization(\_:)

Asks the delegate whether to attempt recovery of world-tracking state after an interruption.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
optional func sessionShouldAttemptRelocalization(_ session: ARSession) -> Bool
```

## Parameters 

`session`  

The session providing information.

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

When ARKit loses track of the device’s position or orientation, ARKit calls sessionShouldAttemptRelocalization(_:) to try to resume the experience where the user left off. This process is called *relocalization*. ARKit relocalizes when it loses access to the camera or other sensors on the device, such as when your app calls pause(), or when the user switches to another app and back.

When relocalization succeeds, your app’s virtual content appears in the same position it was in before the interruption. But if your app fails to relocalize, the world coordinate system and anchor positions are likely out of sync with the real world.

Here are the possible scenarios:

- If by default you don’t implement this function, ARKit spends a few seconds trying to relocalize before restarting your session.

- If you implement this function and return false, ARKit does not attempt to relocalize after an interruption, and the session restarts immediately.

- If you implement this function and return true, you allow the user more time to find the location they were in and resume where they left off, but you’re responsible for restarting the session when it’s prudent to do so.

When you return true, guide the user to facilitate relocalization; for example, by presenting a UI that asks them to return to their previous location. Relocalization works when ARKit recognizes the physical environment it observed before the interruption. If the user does not return to their previous location, the app stays in ARCamera.TrackingState.Reason.relocalizing state indefinitely. It’s important to give the user a way to restart if they choose to. Using ARCoachingOverlayView makes much of this functionality available.

To respond to failed relocalization, call the session’s run(_:options:) method with the resetTracking option. Resetting tracking during relocalization discards all world-tracking state from before the interruption, but keeps world-tracking results obtained during the relocalization attempt.

## See Also

### Handling Interruptions

func sessionWasInterrupted(ARSession)

Tells the delegate that the session has temporarily stopped processing frames and tracking device position.

func sessionInterruptionEnded(ARSession)

Tells the delegate that the session has resumed processing frames and tracking device position.

