

- TabletopKit
-  EntityRenderDelegate 

Protocol

# EntityRenderDelegate

A protocol for the object that renders your entire game using RealityKit.

TabletopKitRealityKitvisionOS 2.0+

``` source
protocol EntityRenderDelegate : TabletopGame.RenderDelegate
```

## Topics

### Getting the root entity

var root: Entity

**Required**

### Rendering the table

func updateRootPose(Pose3D)

## Relationships

### Inherits From

- TabletopGame.RenderDelegate

## See Also

### Rendering the table

func addRenderDelegate(some TabletopGame.RenderDelegate)

func removeRenderDelegate(some TabletopGame.RenderDelegate)

protocol RenderDelegate

A protocol for the object that renders your entire game.

