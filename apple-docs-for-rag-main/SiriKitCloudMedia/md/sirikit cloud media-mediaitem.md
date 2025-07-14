

- SiriKit Cloud Media
-  MediaItem 

Object

# MediaItem

A particular piece of media that an intent references, such as a song, podcast episode, or playlist.

SiriKit Cloud Media 1.0.2+

``` source
object MediaItem
```

## Properties

`identifier`

`string`

 (Required) 

An identifier for the media item that’s stable within the Session and unique among all media of this `type` within this `Session`.

Maximum length: `250`

`title`

`string`

 (Read-only) 

The name of this media item.

Maximum length: `1000`

`artist`

`string`

 (Read-only) 

The performer of this media item.

Maximum length: `1000`

`type`

MediaItemType

 (Required) 

The media item’s type.

## See Also

### Media Items

type MediaReference

A way of identifying the current media item rather than with metadata.

object MediaSearch

A description of the media items the user wants to play, add to a playlist, or express a preference for.

type MediaItemType

Types of media items or media searches.

