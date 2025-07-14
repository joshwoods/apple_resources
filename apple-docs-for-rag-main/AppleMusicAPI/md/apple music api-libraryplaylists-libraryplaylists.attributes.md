

- Apple Music API
- LibraryPlaylists
-  LibraryPlaylists.Attributes 

Object

# LibraryPlaylists.Attributes

The attributes for a library playlist resource.

Apple Music 1.0+

``` source
object LibraryPlaylists.Attributes
```

## Properties

`artwork`

Artwork

The playlist artwork.

`canEdit`

`boolean`

 (Required) 

Indicates whether the playlist is editable.

`dateAdded`

`string`

The date and time the playlist was added to the user’s library.

In YYYY-MM-DDThh:mm:ssZ ISO 8601 format.

`description`

DescriptionAttribute

A description of the playlist.

`hasCatalog`

`boolean`

 (Required) 

Indicates whether the playlist has a representation in the Apple Music catalog.

`name`

`string`

 (Required) 

The localized name of the playlist.

`playParams`

PlayParameters

The value map may be used to initiate playback of available tracks in the playlist.

`isPublic`

`boolean`

 (Required) 

A flag to indicate whether the library playlist is a public playlist.

`trackTypes`

`[string]`

**(Extended)** The resource types that are present in the tracks of the library playlist.

Possible Values: `library-music-videos, library-songs`

## See Also

### Related Objects

object LibraryPlaylists.Relationships

The relationships for a library playlist resource.

