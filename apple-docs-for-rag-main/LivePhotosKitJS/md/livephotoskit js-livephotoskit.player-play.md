

- LivePhotosKit JS
- LivePhotosKit.Player
-  play 

Instance Method

# play

Starts playback if the player is ready, or resumes playback if the player is paused.

LivePhotosKit JS 1.0+

``` source
Boolean play();
```

## Return Value

`true` if the player starts or resumes playback; otherwise, `false`.

## Discussion

If the playback completes, this method fires the `ended` event. If the playback is paused (and not resumed) or stopped, the `ended` event is not fired.

## See Also

### Instance Methods

beginFinishingPlaybackEarly

Clips the duration of the renderer early so that the animation begins to fade back to the photo component earlier than it would ordinarily.

pause

Pauses playback at the current time.

stop

Stops playback and rewinds to the current time of zero.

toggle

Starts playing the video component of Live Photo if the video is paused, or pauses the video if it is playing.

updateSize

Updates the size of the player.

