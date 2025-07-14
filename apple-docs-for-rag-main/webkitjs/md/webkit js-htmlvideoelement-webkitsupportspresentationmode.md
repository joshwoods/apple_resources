

- WebKit JS
- HTMLVideoElement
-  webkitSupportsPresentationMode 

Instance Method

# webkitSupportsPresentationMode

A Boolean value indicating whether the video can be played in presentation mode.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
boolean webkitSupportsPresentationMode(
    VideoPresentationMode mode
);
```

## Discussion

`true` if the device supports presentation mode; otherwise, `false`. This property is also `false` if the meta data is loaded or the `loadedmetadata` event has not fired, and if the files are audio-only.

## See Also

### Displaying Presentation Mode

webkitSetPresentationMode

Sets the presentation mode for video playback.

webkitPresentationMode

A property indicating the presentation mode.

playsInline

A Boolean value indicating whether the video plays inline.

