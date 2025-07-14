

- RealityKit
-  RealityCoordinateSpace 

Protocol

# RealityCoordinateSpace

A 3D coordinate space that exists within a RealityKit hierarchy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
protocol RealityCoordinateSpace
```

## Overview

Any `RealityCoordinateSpaceConverting` can convert spatial data between a SwiftUI `CoordinateSpace` and a `RealityCoordinateSpace`.

## Topics

### Type Properties

static var camera: CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

static var scene: SceneRealityCoordinateSpace

The coordinate space that represents ARKit world space.

## Relationships

### Conforming Types

- AnchorEntity
- BodyTrackedEntity
- CameraRealityCoordinateSpace
- DirectionalLight
- Entity
- ModelEntity
- PerspectiveCamera
- PointLight
- RealityViewContent
- SceneRealityCoordinateSpace
- SpotLight
- TriggerVolume
- ViewAttachmentEntity

## See Also

### Coordinate space conversions

protocol RealityCoordinateSpaceConverting

A value that can be converted between SwiftUI `CoordinateSpace` and RealityKit `Entity`.

struct SceneRealityCoordinateSpace

The coordinate space that represents the center of a RealityKit scene.

struct CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

protocol RealityCoordinateSpaceProjecting

A protocol for coordinate spaces that can project 2D points to and from 3D.

