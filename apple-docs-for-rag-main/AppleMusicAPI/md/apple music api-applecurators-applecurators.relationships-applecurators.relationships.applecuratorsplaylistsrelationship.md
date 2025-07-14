

- Apple Music API
- AppleCurators
- AppleCurators.Relationships
-  AppleCurators.Relationships.AppleCuratorsPlaylistsRelationship 

Object

# AppleCurators.Relationships.AppleCuratorsPlaylistsRelationship

A relationship from the Apple curator to its playlists.

Apple Music 1.0+

``` source
object AppleCurators.Relationships.AppleCuratorsPlaylistsRelationship
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

