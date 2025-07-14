

- Apple Music API
-  Resource 

Object

# Resource

A resource—such as an album, song, or playlist.

Apple Music 1.0+

``` source
object Resource
```

## Properties

`id`

`string`

 (Required) 

Persistent identifier of the resource.

`type`

`string`

 (Required) 

The type of resource.

`href`

`string`

A URL subpath that fetches the resource as the primary object. This member is only present in responses.

`attributes`

Resource.Attributes

Attributes belonging to the resource (can be a subset of the attributes). The members are the names of the attributes defined in the object model.

`relationships`

Resource.Relationships

Relationships belonging to the resource (can be a subset of the relationships). The members are the names of the relationships defined in the object model. See Relationship object for the values of the members.

`meta`

Resource.Meta

Information about the request or response. The members may be any of the endpoint parameters.

`views`

Resource.Views

The relationship views for the resource.

## Discussion

A Resource object may contain just these identifier members: `id`, `type`, `href`, and `meta`.

## Topics

### Related Objects

object Resource.Attributes

Attributes representing the metadata of the resource.

object Resource.Relationships

Relationships belonging to the resource.

### Dictionaries

object Resource.Meta

Information about the request or response.

object Resource.Views

Views belonging to the resource.

## See Also

### Getting Resource and Relationship Information

object Relationship

A to-one or to-many relationship from one resource object to others.

