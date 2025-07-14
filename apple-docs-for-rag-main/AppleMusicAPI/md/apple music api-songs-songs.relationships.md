

- Apple Music API
- Songs
-  Songs.Relationships 

Object

# Songs.Relationships

The relationships for a song resource.

Apple Music 1.0+

``` source
object Songs.Relationships
```

## Properties

`albums`

Songs.Relationships.SongsAlbumsRelationship

The albums associated with the song. By default, `albums` includes identifiers only.

Fetch limits: 10 default, 10 maximum

`artists`

Songs.Relationships.SongsArtistsRelationship

The artists associated with the song. By default, `artists` includes identifiers only.

Fetch limits: 10 default, 10 maximum

`composers`

Songs.Relationships.SongsComposersRelationship

The composers for a catalog song.

`genres`

Songs.Relationships.SongsGenresRelationship

The genres associated with the song. By default, `genres` is not included.

Fetch limits: None

`library`

Songs.Relationships.SongsLibraryRelationship

Library song for a catalog song if added to library.

`music-videos`

Songs.Relationships.SongsMusicVideosRelationship

Music videos for a catalog song.

`station`

Songs.Relationships.SongsStationRelationship

The station associated with the song. By default, `station` is not included.

Fetch limits: None

## Topics

### Related Objects

object Songs.Relationships.SongsAlbumsRelationship

A relationship from the song to its albums.

object Songs.Relationships.SongsArtistsRelationship

A relationship from the song to its artists.

object Songs.Relationships.SongsGenresRelationship

A relationship from the song to its genres.

object Songs.Relationships.SongsComposersRelationship

A relationship from the song to its composers.

object Songs.Relationships.SongsLibraryRelationship

A relationship from the song to its library.

object Songs.Relationships.SongsMusicVideosRelationship

A relationship from the song to its music videos.

object Songs.Relationships.SongsStationRelationship

A relationship from the song to its station.

## See Also

### Related Objects

object Songs.Attributes

The attributes for a song resource.

