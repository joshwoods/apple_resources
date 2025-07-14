

- Apple Music API
- Playlists
-  Playlists.Attributes 

Object

# Playlists.Attributes

The attributes for a playlist resource.

Apple Music 1.0+

``` source
object Playlists.Attributes
```

## Properties

`artwork`

Artwork

The playlist artwork.

`curatorName`

`string`

 (Required) 

The display name of the curator.

`description`

DescriptionAttribute

A description of the playlist.

`isChart`

`boolean`

 (Required) 

Indicates whether the playlist represents a popularity chart.

`lastModifiedDate`

`string`

The date the playlist was last modified.

`name`

`string`

 (Required) 

The localized name of the playlist.

`playlistType`

`string`

 (Required) 

The type of playlist. Possible values are:

Editorial: A playlist created by an Apple Music curator.

External: A playlist created by a non-Apple curator or brand.

Personal-mix: A personalized playlist for an Apple Music user.

Replay: A personalized Apple Music Replay playlist for an Apple Music user.

User-shared: A playlist created and shared by an Apple Music user.

Possible Values: `editorial, external, personal-mix, replay, user-shared`

`playParams`

PlayParameters

The value map may be used to initiate playback of available tracks in the playlist.

`url`

`string`

 (Required) 

The URL for sharing the playlist in Apple Music.

`trackTypes`

`[string]`

**(Extended)** The resource types that are present in the tracks of the playlists.

Possible Values: `music-videos, songs`

## See Also

### Related Objects

object Playlists.Relationships

The relationships for a playlist resource.

object Playlists.Views

The views for a music video resource.

