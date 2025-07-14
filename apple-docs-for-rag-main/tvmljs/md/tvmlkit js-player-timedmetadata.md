

- TVMLKit JS
- Player
-  timedMetadata 

Instance Property

# timedMetadata

An event that is triggered whenever a specified piece of metadata is encountered.

tvOS 9.0+

``` source
attribute  timedMetadata;
```

## Discussion

Specify the metadata this event fires on in the `extraInfo` parameter for the listener. The parameter is an array of keys. Valid key values are: `identifier`, `key`, `stringValue`, and `time`. Passing an empty array or `nil` to observe all timed metadata for HLS streams.

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

timeDidChange

An event that happens at a specified interval.

transportBarVisibilityDidChange

An event that indicates the state of the transport bar has changed.

