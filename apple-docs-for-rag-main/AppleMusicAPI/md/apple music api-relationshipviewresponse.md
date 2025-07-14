

- Apple Music API
-  RelationshipViewResponse 

Object

# RelationshipViewResponse

The response for a direct resource view fetch.

Apple Music 1.0+

``` source
object RelationshipViewResponse
```

## Properties

`attributes`

RelationshipViewResponse.Attributes

The attribute metadata for the view.

`data`

`[`Resource`]`

 (Required) 

A paginated collection of resources in the view.

`meta`

RelationshipViewResponse.Meta

Contextual data about the view.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the view if more exist.

## Topics

### Related Objects

object RelationshipViewResponse.Attributes

The attribute metadata for the view.

object RelationshipViewResponse.Meta

Contextual data about the view.

