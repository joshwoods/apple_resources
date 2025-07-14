

- App Intents
-  EntityQuerySortableByProperty 

Structure

# EntityQuerySortableByProperty

Details about a specific property you use to sort the query results.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EntityQuerySortableByProperty where Entity : AppEntity
```

## Topics

### Creating the sort option

init&lt;Property>(KeyPath&lt;Entity, Property>)

## See Also

### Property-matched queries

protocol EntityPropertyQuery

An interface for locating entities by matching values against one or more of their properties.

struct EntityQueryProperties

A type that provides the properties to include in a property-matched query.

class EntityQueryProperty

An object that provides the supported comparators you use to describe the different ways users can query against a property of an app entity.

Property comparators

Specify the type of comparison to perform during a property-matched query.

struct EntityQuerySortingOptions

The potential properties you can use to sort the results of a query.

struct EntityQuerySort

The properties to use to sort the results when the query runs.

