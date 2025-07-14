

- TVMLKit JS
- Player
-  requestSeekToTime 

Instance Property

# requestSeekToTime

An event that indicates whether a seek-to-time request was accomplished.

tvOS 9.0+

``` source
attribute  requestSeekToTime;
```

## Discussion

This event is called after the left or right edge of the Siri Remote is pressed and released. Use shouldHandleStateChange for press and hold events.

Only a single `requestSeekToTime` listener can be active at a time. If multiple listeners are set to listen for `requestSeekToTime`, only the last one will be updated. The listener is passed an event object with the following attributes:

- `currentTime`—The current playback time in seconds.

- `requestedTime`—The requested playback time in seconds.

- `target`—The event object, which is the Player object.

- `timeStamp`—The time that the event occurred.

- `type`—The name of the event.

The listener must return one of the following values:

- `true`. The seek performed as requested.

- `false` or `null`. The seek was not performed.

- An integer value. The seek will be performed to the stated value and not the initial requested value.

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

