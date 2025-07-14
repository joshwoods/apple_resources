

- Apple Music API
-  AppleCurators 

Object

# AppleCurators

A resource object that represents an Apple curator.

Apple Music 1.0+

``` source
object AppleCurators
```

## Properties

`id`

`string`

 (Required) 

The identifier for the Apple curator.

`type`

`string`

 (Required) 

This value must always be `apple-curators`.

Value: `apple-curators`

`href`

`string`

 (Required) 

The relative location for the Apple curator resource.

`attributes`

AppleCurators.Attributes

The attributes for the Apple curator.

`relationships`

AppleCurators.Relationships

The relationships for the Apple curator.

## Topics

### Related Objects

object AppleCurators.Attributes

The attributes for an Apple curator resource.

object AppleCurators.Relationships

The relationships for an Apple curator resource.

## See Also

### Handling the Response

object AppleCuratorsResponse

The response to a request for Apple curators.

object Curators

A resource object that represents a curator.

object CuratorsResponse

The response to a request for curators.

