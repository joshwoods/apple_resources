

- SwiftUI
- Gesture
-  targetedToEntity(\_:) 

Instance Method

# targetedToEntity(\_:)

Requires this gesture to target an entity or a descendant of entity.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func targetedToEntity(_ entity: Entity) -> some Gesture>
```

## Parameters 

`entity`  

The entity the gesture targets.

## Return Value

A `RealityCoordinateSpaceConverting` value containing the original gesture value along with the targeted entity.

## See Also

### Using a gesture with a RealityKit entity

func targetedToAnyEntity() -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity.

func targetedToEntity(where: QueryPredicate&lt;Entity>) -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity that can be found in the results of the query.

