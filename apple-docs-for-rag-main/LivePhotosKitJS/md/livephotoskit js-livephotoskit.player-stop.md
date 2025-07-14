

- LivePhotosKit JS
- LivePhotosKit.Player
-  stop 

Instance Method

# stop

Stops playback and rewinds to the current time of zero.

LivePhotosKit JS 1.0+

``` source
void stop();
```

## Discussion

After this method is called, the currentTime property is `0`. Like pause, this causes wantsToPlay to become `false`.

## See Also

### Instance Methods

beginFinishingPlaybackEarly

Clips the duration of the renderer early so that the animation begins to fade back to the photo component earlier than it would ordinarily.

pause

Pauses playback at the current time.

play

Starts playback if the player is ready, or resumes playback if the player is paused.

toggle

Starts playing the video component of Live Photo if the video is paused, or pauses the video if it is playing.

updateSize

Updates the size of the player.

