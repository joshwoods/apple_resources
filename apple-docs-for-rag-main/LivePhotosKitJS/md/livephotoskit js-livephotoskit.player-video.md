

- LivePhotosKit JS
- LivePhotosKit.Player
-  video 

Instance Property

# video

The playable `HTMLVideoElement` that the Player consumes to obtain video frame data to render to the screen while animating a Live Photo.

LivePhotosKit JS 1.3+

``` source
attribute HTMLVideoElement video;
```

## Discussion

If this property is not populated by a playable `HTMLVideoElement`, the Player cannot play, but can still render as a photo if `photo` is populated.

You can get a value for this property in one of a few ways:

- Set videoSrc to a string URL and wait for the resulting download and preparation to complete, at which point the property is populated with the resulting `HTMLVideoElement`.

- Set the videoSrc to an `ArrayBuffer` and wait for the resulting preparation to complete, at which point the property is populated with the resulting `HTMLVideoElement`.

- Set the property directly to a fully playable `HTMLVideoElement` whose `canplay` event has fired.

Assigning this property directly causes videoSrc to be cleared and set back to `null`. Moreover, if videoSrc was recently assigned and a network request or asynchronous decoding is still happening, that activity is also canceled.

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

