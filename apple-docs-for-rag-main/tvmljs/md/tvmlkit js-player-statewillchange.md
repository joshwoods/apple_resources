

- TVMLKit JS
- Player
-  stateWillChange 

Instance Property

# stateWillChange

An event that indicates the state of the player is about to change.

tvOS 9.0+

``` source
attribute  stateWillChange;
```

## Discussion

The listener is passed an event object with the following attributes:

- `oldState`—The previous state of the player. Valid values are `playing`, `paused`, and `scanning`.

- `state`—The state that the player is has switched to. Valid values are `playing`, `paused`, and `scanning`.

- `target`—The event object, which is the Player object.

- `timeStamp`—The time that the event occurred.

- `type`—The name of the event.

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

timeBoundaryDidCross

An event that indicates a specific playback time in the media item has been crossed.

timeDidChange

An event that happens at a specified interval.

timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

