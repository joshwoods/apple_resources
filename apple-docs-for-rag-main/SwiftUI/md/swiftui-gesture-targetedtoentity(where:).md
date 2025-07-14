

- SwiftUI
- Gesture
-  targetedToEntity(where:) 

Instance Method

# targetedToEntity(where:)

Requires this gesture to target an entity that can be found in the results of the query.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func targetedToEntity(where query: QueryPredicate) -> some Gesture>
```

## Parameters 

`query`  

A query to filter which entity the gesture targets.

## Return Value

A `RealityCoordinateSpaceConverting` value containing the original gesture value along with the targeted entity.

## See Also

### Using a gesture with a RealityKit entity

func targetedToAnyEntity() -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity.

func targetedToEntity(Entity) -> some Gesture&lt;EntityTargetValue&lt;Self.Value>> 

Requires this gesture to target an entity or a descendant of entity.

