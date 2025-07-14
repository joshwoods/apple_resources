

- Device Management
-  Apps 

Object

# Apps

A resource object that represents an app.

Device Assignment ServicesVPP License Management

``` source
object Apps
```

## Properties

`attributes`

Apps.Attributes

The attributes for the apps resource type.

`href`

`string`

 (Required) 

A relative location for the apps resource.

`id`

`string`

 (Required) 

The identifier for the apps resource.

`relationships`

Apps.Relationships

The relationships from apps to other resources.

`type`

`string`

 (Required) 

The type of the resource. The only allowed value is `apps`.

Value: `apps`

## Topics

### Related Objects

object Apps.Attributes

The attributes for an apps resource.

object Apps.Relationships

The relationships for an apps resource.

## See Also

### Getting common type information

object Artwork

An object that represents artwork.

object DescriptionAttribute

An object that represents a description attribute.

object Genres

A resource object that represents a music genre.

object Books

A resource object that represents a book.

