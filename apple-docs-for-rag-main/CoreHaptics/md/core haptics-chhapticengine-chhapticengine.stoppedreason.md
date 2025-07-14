

- Core Haptics
- CHHapticEngine
-  CHHapticEngine.StoppedReason 

Enumeration

# CHHapticEngine.StoppedReason

The enumeration of reasons the haptic engine stopped running.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
enum StoppedReason
```

## Topics

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

case systemError

A system error stopped the engine.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Haptic Engine Stoppages

var stoppedHandler: CHHapticEngine.StoppedHandler

A closure the haptic engine calls when it stops due to external causes.

typealias StoppedHandler

A typealias for the block that the haptic engine calls after it stops due to an external cause.

