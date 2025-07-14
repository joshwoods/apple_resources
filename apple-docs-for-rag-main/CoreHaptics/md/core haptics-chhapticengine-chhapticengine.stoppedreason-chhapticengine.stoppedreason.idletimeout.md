

- Core Haptics
- CHHapticEngine
- CHHapticEngine.StoppedReason
-  CHHapticEngine.StoppedReason.idleTimeout 

Case

# CHHapticEngine.StoppedReason.idleTimeout

The engine shut down because you’ve enabled automatic shutdown, and the engine reached its idle timeout.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
case idleTimeout
```

## Discussion

If there’s a time-critical pattern to play, restart the engine. Otherwise, do nothing and the engine will automatically restart when the next pattern plays.

Note

Delegating engine restart to the system can add a slight delay to the start of the pattern.

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

case notifyWhenFinished

You’ve asked the system to notify you when it shuts down the engine.

case systemError

A system error stopped the engine.

