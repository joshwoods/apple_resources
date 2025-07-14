

- WebKit JS
- HTMLMediaElement
-  playbackRate 

Instance Property

# playbackRate

The speed that the media resource is playing.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute unrestricted double playbackRate;
```

## Discussion

The value of this property is a multiple of the media resource’s intrinsic speed. If set to `0.0`, a `NOT_SUPPORTED_ERR` DOM exception is raised. The default value is `1.0`. Use this property to create custom controls for playback rate. Values greater than `1.0` fast-forward media and values less than `0.0` rewind. This property can not be set for HTML5 audio/video elements on iOS.

## See Also

### Getting and Setting Properties

autoplay

A Boolean value that determines whether the media resource plays automatically when available.

controls

A Boolean value that determines whether the playback controls appear.

currentTime

The current playback position in seconds.

defaultPlaybackRate

The default rate used to play the media resource.

loop

A Boolean value that determines whether the playback should loop.

muted

A Boolean value that determines whether the audio content should be muted.

preload

A DOMString value that gives a hint to the browser how much of the media should be fetched when the webpage is loaded.

src

The URI address of the media resource to play.

volume

The volume of the audio portion of the media element.

