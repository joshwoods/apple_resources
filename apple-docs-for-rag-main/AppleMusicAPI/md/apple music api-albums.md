

- Apple Music API
-  Albums 

Object

# Albums

A resource object that represents an album.

Apple Music 1.0+

``` source
object Albums
```

## Properties

`id`

`string`

 (Required) 

The identifier for the album.

`type`

`string`

 (Required) 

This value is always `albums`.

Value: `albums`

`href`

`string`

 (Required) 

The relative location for the album resource.

`attributes`

Albums.Attributes

The attributes for the album.

`relationships`

Albums.Relationships

The relationships for the album.

`views`

Albums.Views

The relationship views for the album.

## Mentioned in 

Handling Resource Representation and Relationships

## Topics

### Related Objects

object Albums.Attributes

The attributes for an album resource.

object Albums.Relationships

The relationships for an album resource.

object Albums.Views

The relationship views for an album resource.

## See Also

### Handling the Response

object AlbumsResponse

The response to an albums request.

object LibraryAlbums

A resource object that represents a library album.

object LibraryAlbumsResponse

The response to a library albums request.

