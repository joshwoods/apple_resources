

- TVMLKit JS
- Player
-  shouldHandleStateChange 

Instance Property

# shouldHandleStateChange

An event that indicates a state change request has occurred.

tvOS 9.0+

``` source
attribute  shouldHandleStateChange;
```

## Discussion

This event is called when the user requests a change, but before the change occurs. Only a single `shouldHandleStateChange` listener can be active at a time. If multiple listeners are set to listen for `shouldHandleStateChange`, only the last one will be updated. The listener is passed an event object with the following attributes:

- `duration`—The duration, in seconds, of the asset being played.

- `elapsedTime`—The elapsed time, in seconds, of the asset being played.

- `oldState`—The previous state of the player. Valid values are `playing`, `paused`, and `scanning`.

- `state`—The state that the player is about to switch to. Valid values are `playing`, `paused`, and `scanning`.

- `target`—The event object, which is the Player object.

- `timeStamp`—The time that the event occurred.

- `type`—The name of the event.

The listener must return one of the following values:

- `true`. The state is allowed.

- `false`. The state change is not allowed.

Note

This event occurs after a user has performed an action and needs to be handled as quickly as possible.

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

