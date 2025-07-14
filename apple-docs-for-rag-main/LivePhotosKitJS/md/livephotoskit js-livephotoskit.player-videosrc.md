

- LivePhotosKit JS
- LivePhotosKit.Player
-  videoSrc 

Instance Property

# videoSrc

A reference to the source of the video component of this Live Photo.

LivePhotosKit JS 1.3+

``` source
attribute String,ArrayBuffer videoSrc;
```

## Discussion

Set this property to one of three types of value:

- A string URL

- An `ArrayBuffer` instance that may already be available

- `null` (to clear the Player’s video)

Changing this value causes the video property (the `HTMLVideoElement` consumed by the Player for rendering) to be initially set to `null`. If the new value assigned is a string URL or an `ArrayBuffer`, a round of loading and decoding activity begins, eventually resulting in the video property being populated with the newly loaded video. Only a string URL produces a network request as part of this loading process.

Changing this value while loading activity from a previous assignment is in progress causes the previous loading activity to abort.

Once the file associated with this property is obtained, it is parsed to automatically determine the values of the photoTime and frameTimes properties. These properties must themselves have their values before playback can begin.

Note: If, due to the architecture of your web app or web page, a `` element is available and already sufficiently loaded to be seekable, it might be written directly to the video property. However, when you bypass `videoSrc` in this manner, photoTime and frameTimes are not automatically detected. You have to provide those values by some other means. (see their documentation for more information).

Declarative markup attribute: `data-video-src`

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

