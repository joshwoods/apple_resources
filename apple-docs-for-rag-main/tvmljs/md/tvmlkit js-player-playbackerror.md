

- TVMLKit JS
- Player
-  playbackError 

Instance Property

# playbackError

An event that indicates an error has occurred during playback.

tvOS 10.0+

``` source
attribute  playbackError;
```

## Discussion

The listener is passed an event object with the following attributes:

- `reason`—The localized string describing why the error occurred.

- `shouldStopDueToError`—A boolean that provides a hint as to whether the player should be stopped due to this error.

## See Also

### Responding to Events

mediaItemDidChange

An event notifying the listener that the player changed a media item.

mediaItemWillChange

An event notifying the listener that the player is about to changed a media item.

playbackDidStall

An event that indicates that playback has stalled.

requestSeekToTime

An event that indicates whether a seek-to-time request was accomplished.

shouldChangeToMediaAtIndex

An event that indicates a request to play a media item in a different index is received.

shouldHandleStateChange

An event that indicates a state change request has occurred.

stateDidChange

An event that indicates the state of the player has changed.

stateWillChange

An event that indicates the state of the player is about to change.

timeBoundaryDidCross

An event that indicates a specific playback time in the media item has been crossed.

timeDidChange

An event that happens at a specified interval.

timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

