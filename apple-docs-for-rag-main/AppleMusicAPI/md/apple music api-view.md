

- Apple Music API
-  View 

Object

# View

A to-one or to-many relationship view from one resource object to others representing interesting associations.

Apple Music 1.0+

``` source
object View
```

## Properties

`href`

`string`

A URL subpath that fetches the view resources and attributes as the primary objects. This member is only present in responses.

`next`

`string`

Link to the next page of resources in the view. Contains the `offset` query parameter that specifies the next page. See `Fetch Resources by Page`.

`attributes`

View.Attributes

Attributes specific to the view.

`data`

`[`Resource`]`

 (Required) 

One or more destination objects.

`meta`

View.Meta

Contextual information about the view for the request or response.

## Topics

### Related Objects

object View.Attributes

Attributes representing the metadata of the view.

object View.Meta

Information about the request or response.

