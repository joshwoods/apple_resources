

- Core Haptics
- CHHapticEngine
-  stoppedHandler 

Instance Property

# stoppedHandler

A closure the haptic engine calls when it stops due to external causes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var stoppedHandler: CHHapticEngine.StoppedHandler { get set }
```

## Mentioned in 

Preparing your app to play haptics

## Discussion

External causes that can cause the system to call this closure include audio session interruptions, app suspensions, or system errors. Calling stop(completionHandler:) doesn’t invoke this callback.

Callbacks to this closure don’t occur on the main thread, so handle them in a thread-safe manner.

## See Also

### Handling Haptic Engine Stoppages

typealias StoppedHandler

A typealias for the block that the haptic engine calls after it stops due to an external cause.

enum StoppedReason

The enumeration of reasons the haptic engine stopped running.

