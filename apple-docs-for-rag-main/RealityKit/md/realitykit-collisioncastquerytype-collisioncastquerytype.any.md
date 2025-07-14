

- RealityKit
- CollisionCastQueryType
-  CollisionCastQueryType.any 

Case

# CollisionCastQueryType.any

Report one hit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case any
```

## Discussion

This query type typically executes fastest, but doesn’t guarantee anything about which hit it returns. If you need the hit closest to the origin of the cast, use CollisionCastQueryType.nearest instead.

## See Also

### Collision cast queries

case nearest

Report the closest hit.

case all

Report all hits sorted in ascending order by distance from the cast origin.

