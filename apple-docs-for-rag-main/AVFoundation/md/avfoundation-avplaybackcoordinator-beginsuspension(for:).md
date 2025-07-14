

- AVFoundation
- AVPlaybackCoordinator
-  beginSuspension(for:) 

Instance Method

# beginSuspension(for:)

Tells the coordinator to stop sending playback commands temporarily when the playback object disconnects from the group activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func beginSuspension(for suspensionReason: AVCoordinatedPlaybackSuspension.Reason) -> AVCoordinatedPlaybackSuspension
```

## Parameters 

`suspensionReason`  

The reason for the suspension. Indicate a system-defined value or a custom suspension reason.

## Return Value

A suspension object.

## Discussion

End a suspension by calling its end() or end(proposingNewTime:) method.

## See Also

### Suspending State Coordination

class AVCoordinatedPlaybackSuspension

An object that represents a temporary suspension of coordinated playback.

func expectedItemTime(atHostTime: CMTime) -> CMTime

Returns a time in the current item’s timeline that the coordinator expects to play at the specified host time.

