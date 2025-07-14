

- Core Haptics
- CHHapticEngine
-  CHHapticEngine.StoppedHandler 

Type Alias

# CHHapticEngine.StoppedHandler

A typealias for the block that the haptic engine calls after it stops due to an external cause.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
typealias StoppedHandler = (CHHapticEngine.StoppedReason) -> Void
```

## Discussion

The system calls the stopped handler for when it’s stopped by an external event like an audio session interruption or an auto-shutdown.

Note

The stopped handler isn’t called if you explicitly stop the engine by calling the stop(completionHandler:) method.

## See Also

### Handling Haptic Engine Stoppages

var stoppedHandler: CHHapticEngine.StoppedHandler

A closure the haptic engine calls when it stops due to external causes.

enum StoppedReason

The enumeration of reasons the haptic engine stopped running.

