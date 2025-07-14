

- Apple Music API
-  LibraryAlbums 

Object

# LibraryAlbums

A resource object that represents a library album.

Apple Music 1.0+

``` source
object LibraryAlbums
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library album.

`type`

`string`

 (Required) 

This value is always `library-albums`.

Value: `library-albums`

`href`

`string`

 (Required) 

The relative location for the library album resource.

`attributes`

LibraryAlbums.Attributes

The attributes for the library album.

`relationships`

LibraryAlbums.Relationships

The relationships for the library album.

## Topics

### Related Objects

object LibraryAlbums.Attributes

The attributes for a library album resource.

object LibraryAlbums.Relationships

The relationships for a library album object.

## See Also

### Handling the Response

object Albums

A resource object that represents an album.

object AlbumsResponse

The response to an albums request.

object LibraryAlbumsResponse

The response to a library albums request.

