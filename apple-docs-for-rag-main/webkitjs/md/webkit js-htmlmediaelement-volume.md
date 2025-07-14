

- WebKit JS
- HTMLMediaElement
-  volume 

Instance Property

# volume

The volume of the audio portion of the media element.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute double volume;
```

## Discussion

The value of this property must be in the range from `0.0` (silent) to `1.0` (loudest); otherwise, a `INDEX_SIZE_ERR` DOM exception is raised. The default value is `1.0`.

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

playbackRate

The speed that the media resource is playing.

preload

A DOMString value that gives a hint to the browser how much of the media should be fetched when the webpage is loaded.

src

The URI address of the media resource to play.

