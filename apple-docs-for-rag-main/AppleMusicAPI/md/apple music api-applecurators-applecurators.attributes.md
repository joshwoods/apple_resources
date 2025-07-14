

- Apple Music API
- AppleCurators
-  AppleCurators.Attributes 

Object

# AppleCurators.Attributes

The attributes for an Apple curator resource.

Apple Music 1.0+

``` source
object AppleCurators.Attributes
```

## Properties

`artwork`

Artwork

 (Required) 

The curator artwork.

`editorialNotes`

EditorialNotes

The notes about the curator that appear in the Apple Music catalog.

`kind`

`string`

 (Required) 

The type of curator. Possible values are:

`Curator`: An individual curator entity.

`Genre`: A curator that represents a cohesive music genre.

`Show`: A curator associated with a particular Apple Music show.

Possible Values: `Curator, Genre, Show`

`name`

`string`

 (Required) 

The localized name of the curator.

`shortName`

`string`

The localized shortened name of the curator.

`showHostName`

`string`

The name of the host if `kind` is `Show`.

`url`

`string`

 (Required) 

The URL for sharing the curator in Apple Music.

## See Also

### Related Objects

object AppleCurators.Relationships

The relationships for an Apple curator resource.

