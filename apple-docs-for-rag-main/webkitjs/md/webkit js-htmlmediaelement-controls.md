

- WebKit JS
- HTMLMediaElement
-  controls 

Instance Property

# controls

A Boolean value that determines whether the playback controls appear.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute boolean controls;
```

## Discussion

On the desktop, if `false` (the default), the playback controls do not appear; otherwise, they do appear. On iOS, a native application is used to playback video in full screen; therefore, this property is ignored.

## See Also

### Getting and Setting Properties

autoplay

A Boolean value that determines whether the media resource plays automatically when available.

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

volume

The volume of the audio portion of the media element.

