

- AVFoundation
- AVPlaybackCoordinator
-  expectedItemTime(atHostTime:) 

Instance Method

# expectedItemTime(atHostTime:)

Returns a time in the current item’s timeline that the coordinator expects to play at the specified host time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func expectedItemTime(atHostTime hostClockTime: CMTime) -> CMTime
```

## Parameters 

`hostClockTime`  

The host time to return a player item time for.

## Return Value

A time in the current item’s timeline.

## See Also

### Suspending State Coordination

func beginSuspension(for: AVCoordinatedPlaybackSuspension.Reason) -> AVCoordinatedPlaybackSuspension

Tells the coordinator to stop sending playback commands temporarily when the playback object disconnects from the group activity.

class AVCoordinatedPlaybackSuspension

An object that represents a temporary suspension of coordinated playback.

