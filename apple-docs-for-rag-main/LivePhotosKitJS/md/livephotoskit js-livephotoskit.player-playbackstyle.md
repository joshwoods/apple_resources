

- LivePhotosKit JS
- LivePhotosKit.Player
-  playbackStyle 

Instance Property

# playbackStyle

The style of playback that determines the nature of an animation.

LivePhotosKit JS 1.3+

``` source
attribute LivePhotosKit.PlaybackStyleLiteral playbackStyle;
```

## Discussion

This property can take one of two values:

- `LivePhotosKit.PlaybackStyle.FULL`

- `LivePhotosKit.PlaybackStyle.HINT`

`FULL` refers to the full-featured Live Photo animation consisting of a brief animation forward from the photo. This is followed by a fade transition to the beginning of the video and a subsequent full play through before transitioning back to the photo.

`HINT` refers to a shortened animation that simply plays forward from the photo through the end of the video, before transitioning back to the photo.

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

proactivelyLoadsVideo

A boolean value that indicates whether the Player downloads bytes before the user begins playback.

