

- RealityKit
-  EntityQuery 

Structure

# EntityQuery

An object that retrieves entities from a scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct EntityQuery
```

## Mentioned in 

Implementing scene understanding and reconstruction in your RealityKit app

Implementing systems for entities in a scene

## Overview

Use entity queries to iterate through all entities in a RealityKit scene that meet certain criteria. To specify which entities to retrieve, use a QueryPredicate.

To execute the query, pass it into the scene’s performQuery(_:) method and then iterate over the results.

```
// Build a query to retrieve all anchor components.
let query = EntityQuery(where: .has(AnchorComponent.self)

// Ask the scene to perform the query and iterate over the returned
entities. scene.performQuery(query).forEach { entity in
    // Make any needed changes to entities.
}
```

## Topics

### Creating an entity query

init()

Creates a query that returns all entities in a scene.

init(where: QueryPredicate&lt;Entity>)

Creates a query that returns all entities in a scene that match specific criteria.

## Relationships

### Conforms To

- Sendable

## See Also

### Entity queries

struct QueryPredicate

An object that defines the criteria for an entity query.

struct QueryResult

An object that returns the results of an entity query.

