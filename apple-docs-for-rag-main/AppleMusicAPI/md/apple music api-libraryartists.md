

- Apple Music API
-  LibraryArtists 

Object

# LibraryArtists

A resource object that represents an artist present in a user’s library.

Apple Music 1.0+

``` source
object LibraryArtists
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library artist.

`type`

`string`

 (Required) 

This value is always `library-artists`.

Value: `library-artists`

`href`

`string`

 (Required) 

The relative location for the library artist resource.

`attributes`

LibraryArtists.Attributes

The attributes for the library artist.

`relationships`

LibraryArtists.Relationships

The relationships for the library artist.

## Topics

### Related Objects

object LibraryArtists.Attributes

The attributes for a library artist resource.

object LibraryArtists.Relationships

The relationships for a library artist resource.

## See Also

### Handling the Response

object Artists

A resource object that represents the artist of an album where an artist can be one or more people.

object ArtistsResponse

The response to an artists request.

object LibraryArtistsResponse

The response to a library artists request.

