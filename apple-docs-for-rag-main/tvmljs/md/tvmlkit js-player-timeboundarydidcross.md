

- TVMLKit JS
- Player
-  timeBoundaryDidCross 

Instance Property

# timeBoundaryDidCross

An event that indicates a specific playback time in the media item has been crossed.

tvOS 9.0+

``` source
attribute  timeBoundaryDidCross;
```

## Discussion

This event fires every time the specified playback time is crossed. This can happen multiple times if the user is moving the timing bar back and forth across the boundary. The listener is passed an event object with the following attributes:

- `boundary`—The boundary value that triggered the event when it was crossed.

- `target`—The event object, which is the Player object.

- `timeStamp`—The time that the event occurred.

- `type`—The name of the event.

You must provide an array of numbers, in seconds, as a third parameter to the listener. Each value in the array represents a time boundary as an offset from the beginning of the asset.

## See Also

### Responding to Events

mediaItemDidChange

An event notifying the listener that the player changed a media item.

mediaItemWillChange

An event notifying the listener that the player is about to changed a media item.

playbackDidStall

An event that indicates that playback has stalled.

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

timeDidChange

An event that happens at a specified interval.

timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

