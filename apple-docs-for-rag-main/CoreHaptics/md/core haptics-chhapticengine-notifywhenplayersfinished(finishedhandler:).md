

- Core Haptics
- CHHapticEngine
-  notifyWhenPlayersFinished(finishedHandler:) 

Instance Method

# notifyWhenPlayersFinished(finishedHandler:)

Notifies you when all haptic pattern players have finished playing their haptic patterns.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func notifyWhenPlayersFinished(finishedHandler: @escaping CHHapticEngine.FinishedHandler)
```

## Parameters 

`finishedHandler`  

A closure to execute when all players have finished playback.

## See Also

### Monitoring Finished Playback

typealias FinishedHandler

A type alias for a completion handler to execute after finishing haptic playback.

enum FinishedAction

Possible actions to take after the haptic engine finishes execution.

