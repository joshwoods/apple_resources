

- TabletopKit
- TabletopGame
-  TabletopGame.RenderDelegate 

Protocol

# TabletopGame.RenderDelegate

A protocol for the object that renders your entire game.

visionOS 2.0+

``` source
protocol RenderDelegate : AnyObject
```

## Overview

To provide a renderer, set the TabletopGame object render delegate to an object that conforms to this protocol using the addRenderDelegate(_:) method. Then implement the onUpdate(timeInterval:snapshot:visualState:) protocol method to render the current state of the game.

## Topics

### Rendering the game

func onUpdate(timeInterval: Double, snapshot: TableSnapshot, visualState: TableVisualState)

**Required** Default implementation provided.

func updateRootPose(Pose3D)

**Required** Default implementations provided.

## Relationships

### Inherited By

- EntityRenderDelegate

## See Also

### Rendering the table

func addRenderDelegate(some TabletopGame.RenderDelegate)

func removeRenderDelegate(some TabletopGame.RenderDelegate)

protocol EntityRenderDelegate

A protocol for the object that renders your entire game using RealityKit.

