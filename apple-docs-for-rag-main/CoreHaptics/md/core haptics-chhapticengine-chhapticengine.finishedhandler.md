

- Core Haptics
- CHHapticEngine
-  CHHapticEngine.FinishedHandler 

Type Alias

# CHHapticEngine.FinishedHandler

A type alias for a completion handler to execute after finishing haptic playback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
typealias FinishedHandler = ((any Error)?) -> CHHapticEngine.FinishedAction
```

## See Also

### Monitoring Finished Playback

func notifyWhenPlayersFinished(finishedHandler: CHHapticEngine.FinishedHandler)

Notifies you when all haptic pattern players have finished playing their haptic patterns.

enum FinishedAction

Possible actions to take after the haptic engine finishes execution.

