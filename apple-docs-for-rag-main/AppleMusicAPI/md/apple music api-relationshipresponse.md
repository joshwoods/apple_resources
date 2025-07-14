

- Apple Music API
-  RelationshipResponse 

Object

# RelationshipResponse

The response for a direct resource relationship fetch.

Apple Music 1.0+

``` source
object RelationshipResponse
```

## Properties

`data`

`[`Resource`]`

 (Required) 

A paginated collection of resources in the relationship.

`meta`

RelationshipResponse.Meta

Contextual data about the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

## Topics

### Related Objects

object RelationshipResponse.Meta

Contextual data about the relationship.

