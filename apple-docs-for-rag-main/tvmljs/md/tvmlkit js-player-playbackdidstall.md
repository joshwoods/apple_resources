

- TVMLKit JS
- Player
-  playbackDidStall 

Instance Property

# playbackDidStall

An event that indicates that playback has stalled.

tvOS 10.0+

``` source
attribute  playbackDidStall;
```

## Discussion

The listener is passed an event object with the following attributes:

- `elapsedTime`—The elapsed time, in seconds, of the asset being played.

## See Also

### Responding to Events

mediaItemDidChange

An event notifying the listener that the player changed a media item.

mediaItemWillChange

An event notifying the listener that the player is about to changed a media item.

playbackError

An event that indicates an error has occurred during playback.

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

