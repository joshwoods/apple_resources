

- SiriKit Cloud Media
-  ContentAttributes 

Object

# ContentAttributes

Metadata for some media content.

SiriKit Cloud Media 1.0.2+

``` source
object ContentAttributes
```

## Properties

`albumName`

`string`

The album that contains this media content.

Maximum length: `250`

`artistName`

`string`

The performer of this media content.

Maximum length: `1000`

`artwork`

ContentAttributes.Artwork

The album cover or other imagery.

`composerName`

`string`

The composer of this media content.

Maximum length: `250`

`durationInMillis`

`uint64`

The length of the media content in milliseconds.

`genreNames`

`[string]`

Genres that apply to this media content.

`name`

`string`

The name of the media content.

Maximum length: `250`

`trackNumber`

`uint32`

The media content’s track number within the album.

`contentKeyAssetIdentifier`

`string`

Maximum length: `4000`

## Topics

### Providing Artwork

object ContentAttributes.Artwork

Imagery for media content, such as an album cover.

## See Also

### Providing Queue Items

object Content

A description of a piece of playback content, such as a song, podcast, or advertisement.

type ContentIdentifier

An identifier for a song, podcast, ad, or other media content. The identifier must be stable and unique within a queue.

