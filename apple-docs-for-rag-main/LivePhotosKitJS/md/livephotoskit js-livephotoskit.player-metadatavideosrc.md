

- LivePhotosKit JS
- LivePhotosKit.Player
-  metadataVideoSrc 

Instance Property

# metadataVideoSrc

A string or array buffer that contains metadata about the properties of a Live Photo.

LivePhotosKit JS 1.3+

``` source
attribute String,ArrayBuffer metadataVideoSrc;
```

## Discussion

If you have a video asset that does not include a readable photoTime and/or frameTimes, you can set this property to a string URL or ArrayBuffer referencing the original MOV file that was captured by an iPhone. That file is then parsed in the same manner as those loaded thorough videoSrc. It serves as an alternate source for the photoTime and frameTimes properties if they are not otherwise available.

If this property is set to a URL, the file referred to by the URL is loaded only until the point at which frameTimes and photoTime can be determined from it. The network request is then terminated early to avoid downloading unneeded data. Using this feature to allow the Player to automatically determine frameTimes and/or photoTime may be easier than finding them yourself and providing them manually. However, it comes at the expense of an extra network request incurred by loading the beginning of the file.

You can set this property to an `ArrayBuffer` (for example, videoSrc or photoSrc). However, if you have an `ArrayBuffer` for the original video file, you can set that `ArrayBuffer` here to provide frameTimes and photoTime values. An even simpler alternative is to just use that `ArrayBuffer` as the video source to begin with. (If you supply an `ArrayBuffer` here instead of a URL, there will be no network request, and no performance cost.)

The performance implications of using this property on a small page viewed by audiences with reliable, low-latency connections are probably minimal. However, do not use this approach when performance is critical.

Note

In typical circumstances, you can safely ignore this property.

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

