

- Apple Music API
-  Songs 

Object

# Songs

A resource object that represents a song.

Apple Music 1.0+

``` source
object Songs
```

## Properties

`id`

`string`

 (Required) 

The identifier for the song.

`type`

`string`

 (Required) 

This value is always `songs`.

Value: `songs`

`href`

`string`

 (Required) 

The relative location for the song resource.

`attributes`

Songs.Attributes

The attributes for the song.

`relationships`

Songs.Relationships

The relationships for the song.

## Topics

### Related Objects

object Songs.Attributes

The attributes for a song resource.

object Songs.Relationships

The relationships for a song resource.

## See Also

### Handling the Response

object SongsResponse

The response to a songs request.

object LibrarySongs

A resource object that represents a library song.

object LibrarySongsResponse

The response to a library songs request.

