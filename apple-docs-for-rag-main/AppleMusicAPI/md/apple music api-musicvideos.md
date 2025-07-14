

- Apple Music API
-  MusicVideos 

Object

# MusicVideos

A resource object that represents a music video.

Apple Music 1.0+

``` source
object MusicVideos
```

## Properties

`id`

`string`

 (Required) 

The identifier for the music video.

`type`

`string`

 (Required) 

This value is always `music-videos`.

Value: `music-videos`

`href`

`string`

 (Required) 

The relative location for the music video resource.

`attributes`

MusicVideos.Attributes

The attributes for the music video.

`relationships`

MusicVideos.Relationships

The relationships for the music video.

`views`

MusicVideos.Views

The relationship views for the music video.

## Topics

### Related Objects

object MusicVideos.Attributes

The attributes for a music video resource.

object MusicVideos.Relationships

The relationships for a music video resource.

object MusicVideos.Views

The views for a music video resource.

## See Also

### Handling the Response

object MusicVideosResponse

The response to a music videos request.

object LibraryMusicVideos

A resource object that represents a library music video.

object LibraryMusicVideosResponse

The response to a library music videos request.

