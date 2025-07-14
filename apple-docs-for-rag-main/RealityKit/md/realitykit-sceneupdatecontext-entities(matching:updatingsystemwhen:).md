

- RealityKit
- SceneUpdateContext
-  entities(matching:updatingSystemWhen:) 

Instance Method

# entities(matching:updatingSystemWhen:)

Returns all entities which pass the query predicate of the query.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
func entities(
    matching query: EntityQuery,
    updatingSystemWhen condition: SystemUpdateCondition
) -> QueryResult
```

## Parameters 

`query`  

The query identifying which entities you want to fetch.

`condition`  

How often the System is updated (if the query is not empty).

## Mentioned in 

Implementing systems for entities in a scene

## Discussion

Calling this function can increase the rate at which RealityKit calls the update(context:) method. If `condition` is not met for the current update, this method returns an empty result.

