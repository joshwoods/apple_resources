

- LivePhotosKit JS
- LivePhotosKit.Player
-  photo 

Instance Property

# photo

The renderable, image-bearing DOM element (either an image or a canvas) that the Player consumes to render itself to the screen.

LivePhotosKit JS 1.3+

``` source
attribute HTMLImageElement,HTMLCanvasElement photo;
```

## Discussion

If this property is not populated by an image or canvas, the Player cannot play or render.

You can provide a value for this property in one of several ways:

- Set photoSrc to a string URL and wait for the resulting download and decode to complete, at which point the property is populated with the resulting image.

- Set photoSrc to an `ArrayBuffer` and wait for the decode to complete, at which point the property is populated with the resulting image.

- Set the property directly to a fully loaded `HTMLImageElement` (such that its `complete` property is `true`).

- Set the property directly to an `HTMLCanvasElement` you have prepared, such that its backing store depicts the photo and that the photo is scaled properly.

Assigning this property directly causes photoSrc to be cleared and set back to `null`. Moreover, if photoSrc was recently assigned and a network request or asynchronous decoding is still happening; that activity is also canceled.

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

photoMimeType

The MIME type of a photo asset.

photoSrc

The source of the photo component of the Live Photo.

playbackStyle

The style of playback that determines the nature of an animation.

proactivelyLoadsVideo

A boolean value that indicates whether the Player downloads bytes before the user begins playback.

