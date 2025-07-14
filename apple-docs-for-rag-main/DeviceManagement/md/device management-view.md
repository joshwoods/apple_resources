

- Device Management
-  View 

Object

# View

A view for the resource.

Device Assignment ServicesVPP License Management

``` source
object View
```

## Properties

`attributes`

View.Attributes

The attribute metadata for the view.

`data`

`[`Resource`]`

 (Required) 

A paginated collection of resources in the view.

`href`

`string`

A relative location to fetch the view, if it’s directly fetchable.

`meta`

View.Meta

Contextual data about the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

## Topics

### Objects

object View.Attributes

The attribute metadata for the view.

object View.Meta

Contextual data about the view.

## See Also

### Related Objects

object Resource.Attributes

object Resource.Meta

object Resource.Relationships

object Resource.Views

