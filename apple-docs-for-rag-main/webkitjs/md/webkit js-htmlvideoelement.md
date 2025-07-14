

- WebKit JS
-  HTMLVideoElement 

Class

# HTMLVideoElement

A class representing the HTML `video` element that plays a video in a webpage. Use the HTMLAudioElement class for the HTML `audio` element.

Safari Desktop 10.0+Safari Mobile 3.0+

``` source
interface HTMLVideoElement
```

## Topics

### Getting and Setting Properties

width

The width of the video element in CSS pixels.

height

The height of the video element in CSS pixels.

poster

The URI address of an image file that is shown when no video data is available.

### Getting State

videoWidth

The native width of the video in CSS pixels. (read-only)

videoHeight

The native height of the video in CSS pixels. (read-only)

### Displaying Video Fullscreen

webkitDisplayingFullscreen

A Boolean value indicating whether the video is displaying in fullscreen mode.

webkitEnterFullscreen

Enters fullscreen mode.

webkitExitFullscreen

Exits fullscreen mode.

webkitSupportsFullscreen

A Boolean value indicating whether the video can be played in fullscreen mode.

webkitWirelessVideoPlaybackDisabled

A Boolean value indicating whether wireless video playback is disabled.

webkitEnterFullScreen

Use webkitEnterFullscreen.

webkitExitFullScreen

Use webkitExitFullscreen.

### Displaying Presentation Mode

webkitSetPresentationMode

Sets the presentation mode for video playback.

webkitSupportsPresentationMode

A Boolean value indicating whether the video can be played in presentation mode.

webkitPresentationMode

A property indicating the presentation mode.

playsInline

A Boolean value indicating whether the video plays inline.

## Relationships

### Inherits From

- HTMLMediaElement

