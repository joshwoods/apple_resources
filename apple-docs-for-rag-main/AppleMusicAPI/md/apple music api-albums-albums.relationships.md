

- Apple Music API
- Albums
-  Albums.Relationships 

Object

# Albums.Relationships

The relationships for an album resource.

Apple Music 1.0+

``` source
object Albums.Relationships
```

## Properties

`artists`

Albums.Relationships.AlbumsArtistsRelationship

The artists associated with the album. By default, `artists` includes identifiers only.

Fetch limits: 10 default, 10 maximum

`genres`

Albums.Relationships.AlbumsGenresRelationship

The genres for the album. By default, `genres` not included.

Fetch limits: None

`tracks`

Albums.Relationships.AlbumsTracksRelationship

The songs and music videos on the album. By default, `tracks` includes objects.

Fetch limits: 300 default, 300 maximum

`library`

Albums.Relationships.AlbumsLibraryRelationship

The album in the user’s library for the catalog album, if any.

Fetch limits: None

`record-labels`

Albums.Relationships.AlbumsRecordLabelsRelationship

The record labels for the album

Fetch limits: 10 default, 10 maximum.

## Topics

### Related Objects

object Albums.Relationships.AlbumsArtistsRelationship

A relationship from the album to its artists.

object Albums.Relationships.AlbumsGenresRelationship

A relationship from the album to its genres.

object Albums.Relationships.AlbumsTracksRelationship

A relationship from the album to its tracks.

object Albums.Relationships.AlbumsLibraryRelationship

A relationship from the album to an associated library album.

object Albums.Relationships.AlbumsRecordLabelsRelationship

A relationship from the album to its associated record label.

## See Also

### Related Objects

object Albums.Attributes

The attributes for an album resource.

object Albums.Views

The relationship views for an album resource.

