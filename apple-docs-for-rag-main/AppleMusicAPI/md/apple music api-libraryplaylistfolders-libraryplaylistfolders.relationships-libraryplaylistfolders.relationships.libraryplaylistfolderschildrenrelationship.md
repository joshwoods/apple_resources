

- Apple Music API
- LibraryPlaylistFolders
- LibraryPlaylistFolders.Relationships
-  LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersChildrenRelationship 

Object

# LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersChildrenRelationship

A resource object that represents the children relationship of a library playlist folder.

Apple Music 1.0+

``` source
object LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersChildrenRelationship
```

## Properties

`href`

`string`

The relative location for the children relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[*]`

 (Required) 

The children of the library playlist, if any exist.

Possible types: LibraryPlaylistFolders`, `LibraryPlaylists

## See Also

### Related Objects

object LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersParentRelationship

A resource object that represents the parent relationship of a library playlist folder.

