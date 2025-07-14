

- TVMLKit JS
- Player
-  playbackRate 

Instance Property

# playbackRate

The playback speed.

tvOS 10.0+

``` source
attribute int playbackRate;
```

## Discussion

The default playback speed is `1.0`. Speeds with values smaller than `1.0` play in slow motion. Values higher than `1.0` are time-lapsed. Setting the playback rate to `0` or `1` is not supported, use stop and play respectively.

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

playbackState

The current state of the player.

previous

Immediately begins playing the previous media item in the playlist.

seekToTime

Sets the playback point to a specified time.

stop

Stops the currently playing item and dismisses the player UI.

