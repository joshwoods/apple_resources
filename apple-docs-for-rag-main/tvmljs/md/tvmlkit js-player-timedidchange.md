

- TVMLKit JS
- Player
-  timeDidChange 

Instance Property

# timeDidChange

An event that happens at a specified interval.

tvOS 9.0+

``` source
attribute  timeDidChange;
```

## Discussion

This event fires every time a set number of seconds, starting from the beginning of the media item or 0 seconds, as specified in the `extraInfo` parameter for the listener, occurs. The listener is passed the following attributes:

- `interval`—The desired time interval. This value should be an integer. Floating point values are transformed into integers. The default value is `1`.

- `target`—The event object, which is the Player object.

- `time`—The current playback time, in seconds.

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

stateWillChange

An event that indicates the state of the player is about to change.

timeBoundaryDidCross

An event that indicates a specific playback time in the media item has been crossed.

timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

