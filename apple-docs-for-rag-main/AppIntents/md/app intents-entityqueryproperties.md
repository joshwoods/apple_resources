

- App Intents
-  EntityQueryProperties 

Structure

# EntityQueryProperties

A type that provides the properties to include in a property-matched query.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct EntityQueryProperties where Entity : AppEntity
```

## Overview

Contains all the supported properties a user can query against an entity for a given query. Declare query properties with a block containing all applicable EntityQueryProperty objects.

## Example

```
var properties = QueryProperties {
    Property(\.$myDate) {
        LessThanComparator { /* ... body of mapping transform ... */ }
        GreaterThanComparator { /* ... body of mapping transform ... */ }
    }
    Property(\.$myArray) {
        ContainsComparator { /* ... body of mapping transform ... */ }
    }
}
```

## Topics

### Creating the query properties

enum EntityQueryPropertiesBuilder

A result builder that allows you to declaratively describe the properties to include in a property-matched query.

### Getting the query properties

subscript(Int) -> EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>

### Initializers

init(properties: () -> [EntityQueryPropertyDeclaration&lt;Entity, ComparatorMappingType>])

## See Also

### Property-matched queries

protocol EntityPropertyQuery

An interface for locating entities by matching values against one or more of their properties.

class EntityQueryProperty

An object that provides the supported comparators you use to describe the different ways users can query against a property of an app entity.

Property comparators

Specify the type of comparison to perform during a property-matched query.

struct EntityQuerySortingOptions

The potential properties you can use to sort the results of a query.

struct EntityQuerySortableByProperty

Details about a specific property you use to sort the query results.

struct EntityQuerySort

The properties to use to sort the results when the query runs.

