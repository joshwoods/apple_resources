

- Apple Music API
-  Genres 

Object

# Genres

A resource object that represents a music genre.

Apple Music 1.0+

``` source
object Genres
```

## Properties

`id`

`string`

 (Required) 

The identifier for the genre.

`type`

`string`

 (Required) 

This value must always be `genres`.

Value: `genres`

`href`

`string`

 (Required) 

The relative location for the genre resource.

`attributes`

Genres.Attributes

The attributes for the genre.

## Topics

### Related Objects

object Genres.Attributes

The attributes for a genre resource.

## See Also

### Handling the Response

object GenresResponse

The response to a genres request.

