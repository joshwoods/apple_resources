

- WebKit JS
- HTMLMediaElement
-  currentTime 

Instance Property

# currentTime

The current playback position in seconds.

Safari Desktop 3.1+Safari Mobile 3.0+

``` source
attribute unrestricted double currentTime;
```

## Discussion

When you set this property, the media play head moves to the new location. An `INVALID_STATE_ERR` DOM exception is raised if there is no selected media resource when you set this property. An `INDEX_SIZE_ERR` DOM exception is raised if the specified time is not within the start and end times.

## See Also

### Getting and Setting Properties

autoplay

A Boolean value that determines whether the media resource plays automatically when available.

controls

A Boolean value that determines whether the playback controls appear.

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

