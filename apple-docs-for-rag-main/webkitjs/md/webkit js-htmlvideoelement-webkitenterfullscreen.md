

- WebKit JS
- HTMLVideoElement
-  webkitEnterFullscreen 

Instance Method

# webkitEnterFullscreen

Enters fullscreen mode.

Safari Desktop 5.0+Safari Mobile 4.2+

``` source
void webkitEnterFullscreen();
```

## Discussion

This method throws an exception if the element is not allowed to enter fullscreen—that is, if webkitSupportsFullscreen is `false`.

## See Also

### Displaying Video Fullscreen

webkitDisplayingFullscreen

A Boolean value indicating whether the video is displaying in fullscreen mode.

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

