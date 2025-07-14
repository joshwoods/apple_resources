

- Apple Music API
- Curators
- Curators.Relationships
-  Curators.Relationships.CuratorsPlaylistsRelationship 

Object

# Curators.Relationships.CuratorsPlaylistsRelationship

A relationship from the curator to its playlists.

Apple Music 1.0+

``` source
object Curators.Relationships.CuratorsPlaylistsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`Playlists`]`

 (Required) 

The playlists for the curator.

