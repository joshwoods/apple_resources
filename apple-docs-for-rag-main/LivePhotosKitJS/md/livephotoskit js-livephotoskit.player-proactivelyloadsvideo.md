

- LivePhotosKit JS
- LivePhotosKit.Player
-  proactivelyLoadsVideo 

Instance Property

# proactivelyLoadsVideo

A boolean value that indicates whether the Player downloads bytes before the user begins playback.

LivePhotosKit JS 1.3+

``` source
attribute Boolean proactivelyLoadsVideo;
```

## Discussion

Whether or not the Player downloads bytes at the provided videoSrc before the user begins playback.

If there are many Players on a page, a value of `false` enables configuration of videoSrc on all Players without forcing expensive downloads of each Player’s video asset.

If there are few Players on a page, a value of `true` decreases the warmup and loading time necessary after an attempt to initiate playback before playback actually begins.

This tradeoff is left to the developer, but in the interests of out-of-the-box scalability, this property defaults to `false`.

Declarative markup attribute: `data-proactively-loads-video`

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

