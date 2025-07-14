

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.engineDestroyed 

Case

# CHHapticEngine.StoppedReason.engineDestroyed

The system destroyed the engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case engineDestroyed
```

## Discussion

This reason typically indicates a programming error. Maintain a strong reference to the engine to for as long as you need to execute haptics.

## See Also

### Stopped Reasons

case audioSessionInterrupt

The system interrupted the audio session.

case applicationSuspended

The system suspended your app.

case gameControllerDisconnect

The engine stopped because the associated game controller disconnected from the device.

case idleTimeout

The engine shut down because you’ve enabled automatic shutdown, and the engine reached its idle timeout.

case notifyWhenFinished

You’ve asked the system to notify you when it shuts down the engine.

case systemError

A system error stopped the engine.

