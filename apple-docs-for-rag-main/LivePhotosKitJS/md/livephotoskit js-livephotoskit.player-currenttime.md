

- LivePhotosKit JS
- LivePhotosKit.Player
-  currentTime 

Instance Property

# currentTime

The current time, in seconds, of the play head.

LivePhotosKit JS 1.0+

``` source
readonly attribute Number currentTime;
```

## Discussion

Setting this property moves the play head synchronously to the specified time.

Allowable values are floating points between `0` and duration. A value that places the play head between frames shows a weighted average of the two frames.

If the playback style is FULL a value of `0` corresponds to the at-rest view of the full-resolution photo. As `currentTime` increases, the Live Photo animation will be played back according to the playback style.

Because the required frames might not be decoded, setting `currentTime` could fail. In this case, `currentTime` will not take on its just-assigned value. Setting `currentTime` again to the same value in the near future will most likely succeed. There is no asynchronous callback to test for when the missing requirements for a particular `currentTime` value become available.

## See Also

### Instance Properties

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

proactivelyLoadsVideo

A boolean value that indicates whether the Player downloads bytes before the user begins playback.

