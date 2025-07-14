

- RealityKit
- PortalComponent
-  targetEntity 

Instance Property

# targetEntity

The root entity for the portal’s target world.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var targetEntity: Entity? { get set }
```

## Discussion

When the target entity is valid and has a WorldComponent, the portal renders with the target entity and its hierarchy tree.

When the target entity doesn’t have a WorldComponent, the portal doesn’t render.

