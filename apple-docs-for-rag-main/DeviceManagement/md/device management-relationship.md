

- Device Management
-  Relationship 

Object

# Relationship

A to-one or to-many relationship from one resource object to others.

Device Assignment ServicesVPP License Management

``` source
object Relationship
```

## Properties

`data`

`[`Resource`]`

 (Required) 

A paginated collection of resources in the relationship.

`href`

`string`

A relative location to fetch the relationship, if it may be fetched directly.

`meta`

Relationship.Meta

Contextual data about the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

## Topics

### Related Objects

object Relationship.Meta

## See Also

### Getting resource and relationship information

object Resource

A resource such as an app or book.

