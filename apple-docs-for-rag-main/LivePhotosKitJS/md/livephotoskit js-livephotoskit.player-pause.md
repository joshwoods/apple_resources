

- LivePhotosKit JS
- LivePhotosKit.Player
-  pause 

Instance Method

# pause

Pauses playback at the current time.

LivePhotosKit JS 1.0+

``` source
void pause();
```

## Discussion

This ensures that wantsToPlay is `false`, meaning that if loading activity completes, playback will not begin spuriously.

If the Player is already not playing, then, aside from maintaining the wantsToPlay value, this does nothing.

To resume playback, call the play or toggle method.

## See Also

### Instance Methods

beginFinishingPlaybackEarly

Clips the duration of the renderer early so that the animation begins to fade back to the photo component earlier than it would ordinarily.

play

Starts playback if the player is ready, or resumes playback if the player is paused.

stop

Stops playback and rewinds to the current time of zero.

toggle

Starts playing the video component of Live Photo if the video is paused, or pauses the video if it is playing.

updateSize

Updates the size of the player.

