

- WebKit JS
- HTMLVideoElement
-  webkitSupportsFullscreen 

Instance Property

# webkitSupportsFullscreen

A Boolean value indicating whether the video can be played in fullscreen mode.

Safari Desktop 5.0+Safari Mobile 4.0+

``` source
readonly attribute boolean webkitSupportsFullscreen;
```

## Discussion

`true` if the device supports fullscreen mode; otherwise, `false`. This property is also `false` if the meta data is loaded or the `loadedmetadata` event has not fired, and if the files are audio-only.

## See Also

### Displaying Video Fullscreen

webkitDisplayingFullscreen

A Boolean value indicating whether the video is displaying in fullscreen mode.

webkitEnterFullscreen

Enters fullscreen mode.

webkitExitFullscreen

Exits fullscreen mode.

webkitWirelessVideoPlaybackDisabled

A Boolean value indicating whether wireless video playback is disabled.

webkitEnterFullScreen

Use webkitEnterFullscreen.

webkitExitFullScreen

Use webkitExitFullscreen.

