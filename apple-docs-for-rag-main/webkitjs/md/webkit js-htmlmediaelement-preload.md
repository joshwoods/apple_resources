

- WebKit JS
- HTMLMediaElement
-  preload 

Instance Property

# preload

A DOMString value that gives a hint to the browser how much of the media should be fetched when the webpage is loaded.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute DOMString preload;
```

## Discussion

Possible values are `auto`, `metadata`, and `none`. The attribute defaults to `auto`, suggesting to the browser the server is able to provide the media for immediate and agressive downloading. The `metadata` value suggests minimal server interaction to retrieve only metadata and the first frames of the media resource, while `none` suggests no server interaction is needed. These `preload` values can be changed dynamically. There is no guarantee that you get the behavior that you request.

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

src

The URI address of the media resource to play.

volume

The volume of the audio portion of the media element.

