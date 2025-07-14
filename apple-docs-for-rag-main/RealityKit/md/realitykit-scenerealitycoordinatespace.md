

- RealityKit
-  SceneRealityCoordinateSpace 

Structure

# SceneRealityCoordinateSpace

The coordinate space that represents the center of a RealityKit scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct SceneRealityCoordinateSpace
```

## Overview

The center, or origin, of a RealityKit scene varies depending on the platform and context:

visionOS (Window or Volume)  
The origin is a point that extends outward from the window, or upward from the volume.

visionOS (Immersive Space)  
The origin is the ARKit world origin, which does not directly relate to any specific RealityView, but rather to the broader immersive environment.

macOS and iOS (Non-AR)  
The origin is a point behind the RealityView. Here, the RealityView acts as a window through which you can view the scene, and the scene’s origin is placed behind this by default, giving depth to the scene.

iOS (AR Mode)  
Similar to the Immersive Space in visionOS, ARKit determines the world origin, and does not directly relate to the RealityView position.

Note

This object is equivalent to scene.

## Topics

### Initializers

init()

Creates a scene coordinate space.

### Default Implementations

RealityCoordinateSpace Implementations

## Relationships

### Conforms To

- RealityCoordinateSpace

## See Also

### Coordinate space conversions

protocol RealityCoordinateSpaceConverting

A value that can be converted between SwiftUI `CoordinateSpace` and RealityKit `Entity`.

struct CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

protocol RealityCoordinateSpace

A 3D coordinate space that exists within a RealityKit hierarchy.

protocol RealityCoordinateSpaceProjecting

A protocol for coordinate spaces that can project 2D points to and from 3D.

