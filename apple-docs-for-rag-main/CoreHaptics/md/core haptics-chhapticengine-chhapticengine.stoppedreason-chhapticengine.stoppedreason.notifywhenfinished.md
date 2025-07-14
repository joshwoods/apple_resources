

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.notifyWhenFinished 

Case

# CHHapticEngine.StoppedReason.notifyWhenFinished

You’ve asked the system to notify you when it shuts down the engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case notifyWhenFinished
```

## Discussion

Restart the engine before starting another pattern player.

## See Also

### Stopped Reasons

case audioSessionInterrupt

The system interrupted the audio session.

case applicationSuspended

The system suspended your app.

case engineDestroyed

The system destroyed the engine.

case gameControllerDisconnect

The engine stopped because the associated game controller disconnected from the device.

case idleTimeout

The engine shut down because you’ve enabled automatic shutdown, and the engine reached its idle timeout.

case systemError

A system error stopped the engine.

