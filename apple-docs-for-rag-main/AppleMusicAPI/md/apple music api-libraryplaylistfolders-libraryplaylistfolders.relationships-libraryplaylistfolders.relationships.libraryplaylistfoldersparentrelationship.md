

- Apple Music API
- LibraryPlaylistFolders
- LibraryPlaylistFolders.Relationships
-  LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersParentRelationship 

Object

# LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersParentRelationship

A resource object that represents the parent relationship of a library playlist folder.

Apple Music 1.0+

``` source
object LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersParentRelationship
```

## Properties

`href`

`string`

The relative location for the parent relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`LibraryPlaylistFolders`]`

 (Required) 

The parent of the library playlist, if it exists.

## See Also

### Related Objects

object LibraryPlaylistFolders.Relationships.LibraryPlaylistFoldersChildrenRelationship

A resource object that represents the children relationship of a library playlist folder.

