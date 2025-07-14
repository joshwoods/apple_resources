

- LivePhotosKit JS
- LivePhotosKit.Player
-  videoMimeType 

Instance Property

# videoMimeType

The MIME type of the video asset.

LivePhotosKit JS 1.3+

``` source
attribute String videoMimeType;
```

## Discussion

The `MIME` type of the video asset, either as detected from a network request for the asset (if it was provided as a URL on videoSrc) or as provided by the developer prior to assigning a prepared `ArrayBuffer` to videoSrc.

This property, while writable, behaves as read-only if the video was obtained through a network request to a string URL set on videoSrc. In this case, writes to this property are ignored.

However, if the intent is to provide the video by assigning an already-loaded `ArrayBuffer` to videoSrc, you must set this property to the correct MIME type beforehand.

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

