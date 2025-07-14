

- RealityKit
- CollisionCastQueryType
-  CollisionCastQueryType.nearest 

Case

# CollisionCastQueryType.nearest

Report the closest hit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case nearest
```

## Discussion

If you only want to test if a hit occurs and don’t care about which hit out of multiple possible hits is returned, use CollisionCastQueryType.any instead because it typically executes faster.

## See Also

### Collision cast queries

case all

Report all hits sorted in ascending order by distance from the cast origin.

case any

Report one hit.

