

- Apple Music API
-  LibraryMusicVideos 

Object

# LibraryMusicVideos

A resource object that represents a library music video.

Apple Music 1.0+

``` source
object LibraryMusicVideos
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library music video.

`type`

`string`

 (Required) 

This value is always `library-music-videos`.

Value: `library-music-videos`

`href`

`string`

 (Required) 

The relative location for the library music video resource.

`attributes`

LibraryMusicVideos.Attributes

The attributes for the library music video.

`relationships`

LibraryMusicVideos.Relationships

The relationships for the library music video.

## Topics

### Related Objects

object LibraryMusicVideos.Attributes

The attributes for the library music videos resource type.

object LibraryMusicVideos.Relationships

The relationships from library music videos to other resources.

## See Also

### Handling the Response

object MusicVideos

A resource object that represents a music video.

object MusicVideosResponse

The response to a music videos request.

object LibraryMusicVideosResponse

The response to a library music videos request.

