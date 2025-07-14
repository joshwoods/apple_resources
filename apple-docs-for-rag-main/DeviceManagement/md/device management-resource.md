

- Device Management
-  Resource 

Object

# Resource

A resource such as an app or book.

Device Assignment ServicesVPP License Management

``` source
object Resource
```

## Properties

`attributes`

Resource.Attributes

The attribute metadata for the resource.

`href`

`string`

The relative location for the resource, if it may be fetched directly.

`id`

`string`

 (Required) 

The identifier of the resource.

`meta`

Resource.Meta

Contextual data about the resource.

`relationships`

Resource.Relationships

The relationships for the resource.

`type`

`string`

 (Required) 

The type of the resource.

`views`

Resource.Views

The views for the resource.

## Topics

### Related Objects

object View

A view for the resource.

object Resource.Attributes

object Resource.Meta

object Resource.Relationships

object Resource.Views

## See Also

### Getting resource and relationship information

object Relationship

A to-one or to-many relationship from one resource object to others.

