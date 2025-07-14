

- LivePhotosKit JS
- LivePhotosKit.Player
-  wantsToPlay 

Instance Property

# wantsToPlay

A boolean that indicates whether the Player has been instructed to play.

LivePhotosKit JS 1.3+

``` source
readonly attribute Boolean wantsToPlay;
```

## Discussion

This property indicates whether the Player has been instructed to play. If true, the Player has been instructed to play, although it may not actually be playing. This occurs when the user or developer has invoked play without all the required resources having loaded yet. When the resources are done loading, if `wantsToPlay` is still `true`, playback begins automatically.

## See Also

### Instance Properties

currentTime

The current time, in seconds, of the play head.

duration

The duration, in seconds, of the entire Live Photo.

photoHeight

The height, in pixels, of the photo component.

photoTime

The nominated time, in seconds, of where the photo component should be within the Live Photo video component.

photoWidth

The width, in pixels, of the photo component.

canPlay

A Boolean value that indicates whether the Player is able to begin playback.

errors

An array of errors that occurred when attempting to load resources.

frameTimes

An array of timestamps for each second from the beginning of a Live Photo for which the frames reside in the Live Photo.

isPlaying

A Boolean value that indicates whether or not the Player is playing.

loadProgress

A numeric value that indicates the progress of loading the Live Photo.

metadataVideoSrc

A string or array buffer that contains metadata about the properties of a Live Photo.

photo

The renderable, image-bearing DOM element (either an image or a canvas) that the Player consumes to render itself to the screen.

photoMimeType

The MIME type of a photo asset.

photoSrc

The source of the photo component of the Live Photo.

playbackStyle

The style of playback that determines the nature of an animation.

