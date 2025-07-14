

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.systemError 

Case

# CHHapticEngine.StoppedReason.systemError

A system error stopped the engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case systemError
```

## Mentioned in 

Preparing your app to play haptics

## Discussion

Your app should attempt to restart the engine. If the restart attempt fails multiple times, treat the condition as fatal.

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

case notifyWhenFinished

You’ve asked the system to notify you when it shuts down the engine.

