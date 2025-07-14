

- LivePhotosKit JS
- LivePhotosKit.Player
-  frameTimes 

Instance Property

# frameTimes

An array of timestamps for each second from the beginning of a Live Photo for which the frames reside in the Live Photo.

LivePhotosKit JS 1.3+

``` source
attribute Number[],string frameTimes;
```

## Discussion

The frameTimes array allows the Player to crossfade between video frames during playback.

This value is required to properly play the Live Photo; without it, the Player cannot play.

The player does its best to make it as easy as possible to populate this value. There are a few ways to provide it:

- Assign videoSrc, and use any MPEG-4 or MOV file. The value is read from the video and populated automatically as part of the loading process.

- Provide a URL or `ArrayBuffer` for the original QuickTime MOV to the metadataVideoSrc property. The asset is loaded just far enough to provide the value automatically. Note that this is a convenience, and for performance-critical uses, you may wish to avoid incurring the extra network request.

- If neither of the previous options works, assign the value manually. You can assign it as either an array of floating-point numbers or as a comma-delimited string of decimal values.

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

