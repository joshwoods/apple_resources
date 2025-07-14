

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.applicationSuspended 

Case

# CHHapticEngine.StoppedReason.applicationSuspended

The system suspended your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case applicationSuspended
```

## Discussion

This condition occurs if the system suspended your app while it was in the background. Restart the engine when your app returns to the foreground to ensure proper haptic playback.

## See Also

### Stopped Reasons

case audioSessionInterrupt

The system interrupted the audio session.

case engineDestroyed

The system destroyed the engine.

case gameControllerDisconnect

The engine stopped because the associated game controller disconnected from the device.

case idleTimeout

The engine shut down because you’ve enabled automatic shutdown, and the engine reached its idle timeout.

case notifyWhenFinished

You’ve asked the system to notify you when it shuts down the engine.

case systemError

A system error stopped the engine.

