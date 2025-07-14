

- Apple Music API
-  Artists 

Object

# Artists

A resource object that represents the artist of an album where an artist can be one or more people.

Apple Music 1.0+

``` source
object Artists
```

## Properties

`id`

`string`

 (Required) 

The identifier for the artist.

`type`

`string`

 (Required) 

This value is always `artists`.

Value: `artists`

`href`

`string`

 (Required) 

The relative location for the artist resource.

`attributes`

Artists.Attributes

The attributes for the artist.

`relationships`

Artists.Relationships

The relationships for the artist.

`views`

Artists.Views

The views for associations between artists and other resources.

## Mentioned in 

Handling Resource Representation and Relationships

## Topics

### Related Objects

object Artists.Attributes

The attributes for an artist resource.

object Artists.Relationships

The relationships for an artist resource.

object Artists.Views

The views for associations between artists and other resources.

## See Also

### Handling the Response

object ArtistsResponse

The response to an artists request.

object LibraryArtists

A resource object that represents an artist present in a user’s library.

object LibraryArtistsResponse

The response to a library artists request.

