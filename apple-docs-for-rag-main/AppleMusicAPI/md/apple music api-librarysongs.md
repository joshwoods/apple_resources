

- Apple Music API
-  LibrarySongs 

Object

# LibrarySongs

A resource object that represents a library song.

Apple Music 1.0+

``` source
object LibrarySongs
```

## Properties

`id`

`string`

 (Required) 

The identifier for the library song.

`type`

`string`

 (Required) 

This value is always `library-songs`.

Value: `library-songs`

`href`

`string`

 (Required) 

The relative location for the library song resource.

`attributes`

LibrarySongs.Attributes

The attributes for the library song.

`relationships`

LibrarySongs.Relationships

The relationships for the library song.

## Topics

### Related Objects

object LibrarySongs.Attributes

The attributes for a library song resource.

object LibrarySongs.Relationships

The relationships for a library song resource.

## See Also

### Handling the Response

object Songs

A resource object that represents a song.

object SongsResponse

The response to a songs request.

object LibrarySongsResponse

The response to a library songs request.

