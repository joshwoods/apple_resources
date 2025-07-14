

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.audioSessionInterrupt 

Case

# CHHapticEngine.StoppedReason.audioSessionInterrupt

The system interrupted the audio session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case audioSessionInterrupt
```

## Discussion

Audio session interruptions occur due to interactions with other audio apps. For example, the system interrupts music playback when a user receives a phone call. When an interruption occurs, restart the engine before it starts another pattern player.

## See Also

### Stopped Reasons

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

case systemError

A system error stopped the engine.

