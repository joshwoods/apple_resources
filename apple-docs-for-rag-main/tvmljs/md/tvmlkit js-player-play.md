

- TVMLKit JS
- Player
-  play 

Instance Method

# play

Plays the currently selected media item.

tvOS 9.0+

``` source
void play();
```

## Discussion

This function displays the player onscreen if the player is not currently displayed and a video is played. For audio, this function will display the player only the first time audio is played. To display the player for audio after the first time, use the present function. Only a single player can be active at a time. Calling the `play` function on a Player object will stop any players currently playing.

## See Also

### Controlling Playback

changeToMediaAtIndex

Immediately begins playing the media item at the specified index in the playlist.

pause

Pauses the currently playing media item.

next

Immediately begins playing the next media item in the playlist.

playbackState

The current state of the player.

playbackRate

The playback speed.

previous

Immediately begins playing the previous media item in the playlist.

seekToTime

Sets the playback point to a specified time.

stop

Stops the currently playing item and dismisses the player UI.

