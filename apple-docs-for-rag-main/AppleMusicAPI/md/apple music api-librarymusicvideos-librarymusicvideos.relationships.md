

- Apple Music API
- LibraryMusicVideos
-  LibraryMusicVideos.Relationships 

Object

# LibraryMusicVideos.Relationships

The relationships from library music videos to other resources.

Apple Music 1.0+

``` source
object LibraryMusicVideos.Relationships
```

## Properties

`albums`

LibraryMusicVideos.Relationships.LibraryMusicVideosAlbumsRelationship

The library albums associated with the music video. By default, `albums` not included.

Fetch limits: 10 default, 10 maximum.

`artists`

LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship

The library artists associated with the music video. By default, `artists` not included.

Fetch limits: 10 default, 10 maximum.

`catalog`

LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship

The music video in the Apple Music catalog the library music video is associated with, when known.

Fetch limits: None (associated with at most one catalog music video).

## Topics

### Related Objects

object LibraryMusicVideos.Relationships.LibraryMusicVideosAlbumsRelationship

A relationship from the library music video to its albums in the library.

object LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship

A relationship from the library music video to its artists in the library.

object LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship

A relationship from the library music video to its associated catalog content.

## See Also

### Related Objects

object LibraryMusicVideos.Attributes

The attributes for the library music videos resource type.

