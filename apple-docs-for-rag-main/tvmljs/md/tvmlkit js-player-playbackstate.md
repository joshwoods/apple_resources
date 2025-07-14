

- TVMLKit JS
- Player
-  playbackState 

Instance Property

# playbackState

The current state of the player.

tvOS 9.0+

``` source
readonly attribute String playbackState;
```

## Discussion

This property can contain the following valid values: `begin`, `end`, `loading`, `playing`, `paused`, and `scanning`.

## See Also

### Controlling Playback

changeToMediaAtIndex

Immediately begins playing the media item at the specified index in the playlist.

pause

Pauses the currently playing media item.

next

Immediately begins playing the next media item in the playlist.

play

Plays the currently selected media item.

playbackRate

The playback speed.

previous

Immediately begins playing the previous media item in the playlist.

seekToTime

Sets the playback point to a specified time.

stop

Stops the currently playing item and dismisses the player UI.

