

- TVMLKit JS
- Player
-  seekToTime 

Instance Method

# seekToTime

Sets the playback point to a specified time.

tvOS 9.0+

``` source
void seekToTime(
    in int time
);
```

## Parameters 

`time`  

The time, in seconds from the beginning of media item, that play begins.

## Discussion

Use this function to change where playback for a media item begins. The time where playback begins is passed, in seconds, by the `time` parameter. For example, to start a media item 5 minutes into playback, set the `time` parameter to 300.

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

playbackRate

The playback speed.

previous

Immediately begins playing the previous media item in the playlist.

stop

Stops the currently playing item and dismisses the player UI.

