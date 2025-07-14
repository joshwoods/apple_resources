

- Apple Music API
- Artists
-  Artists.Relationships 

Object

# Artists.Relationships

The relationships for an artist resource.

Apple Music 1.0+

``` source
object Artists.Relationships
```

## Properties

`albums`

Artists.Relationships.ArtistsAlbumsRelationship

The albums associated with the artist. By default, `albums` includes identifiers only.

Fetch limits: 25 default, 100 maximum

`genres`

Artists.Relationships.ArtistsGenresRelationship

The genres associated with the artist. By default, `genres` not included.

Fetch limits: None

`music-videos`

Artists.Relationships.ArtistsMusicVideosRelationship

The music videos associated with the artist. By default, `musicVideos` not included.

Fetch limits: 25 default, 100 maximum

`playlists`

Artists.Relationships.ArtistsPlaylistsRelationship

The playlists associated with the artist. By default, `playlists` not included.

Fetch limits: 10 default, 10 maximum

`station`

Artists.Relationships.ArtistsStationRelationship

The station associated with the artist. By default, station not included.

Fetch limits: None (one station).

## Topics

### Related Objects

object Artists.Relationships.ArtistsAlbumsRelationship

A relationship from the artist to its albums.

object Artists.Relationships.ArtistsGenresRelationship

A relationship from the artist to its genres.

object Artists.Relationships.ArtistsMusicVideosRelationship

A relationship from the artist to its music videos.

object Artists.Relationships.ArtistsPlaylistsRelationship

A relationship from the artist to its playlists.

object Artists.Relationships.ArtistsStationRelationship

A relationship from the artist to its station.

## See Also

### Related Objects

object Artists.Attributes

The attributes for an artist resource.

object Artists.Views

The views for associations between artists and other resources.

