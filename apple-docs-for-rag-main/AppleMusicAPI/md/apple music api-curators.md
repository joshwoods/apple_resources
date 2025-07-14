

- Apple Music API
-  Curators 

Object

# Curators

A resource object that represents a curator.

Apple Music 1.0+

``` source
object Curators
```

## Properties

`id`

`string`

 (Required) 

The identifier for the curator.

`type`

`string`

 (Required) 

This value must always be `curators`.

Value: `curators`

`href`

`string`

 (Required) 

The relative location for the curator resource.

`attributes`

Curators.Attributes

The attributes for the curator.

`relationships`

Curators.Relationships

The relationships for the curator.

## Topics

### Related Objects

object Curators.Attributes

The attributes for a curator resource.

object Curators.Relationships

The relationships for a curator resource.

## See Also

### Handling the Response

object AppleCurators

A resource object that represents an Apple curator.

object AppleCuratorsResponse

The response to a request for Apple curators.

object CuratorsResponse

The response to a request for curators.

