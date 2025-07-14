

- RealityKit
-  RealityCoordinateSpaceProjecting 

Protocol

# RealityCoordinateSpaceProjecting

A protocol for coordinate spaces that can project 2D points to and from 3D.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
protocol RealityCoordinateSpaceProjecting
```

## Topics

### Instance Methods

func entities(at: CGPoint, in: some CoordinateSpaceProtocol) -> [Entity]

Finds all the hit entities when projecting a ray from a starting point.

**Required**

func entity(at: CGPoint, in: some CoordinateSpaceProtocol) -> Entity?

Finds the first entity hit when projecting a ray from a starting point.

**Required**

func hitTest(point: CGPoint, in: some CoordinateSpaceProtocol, query: CollisionCastQueryType, mask: CollisionGroup) -> [CollisionCastHit]

Searches the scene for entities at the specified point in the view.

**Required**

func project(point: SIMD3&lt;Float>, to: some CoordinateSpaceProtocol) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the reality view.

**Required**

func ray(through: CGPoint, in: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> (origin: SIMD3&lt;Float>, direction: SIMD3&lt;Float>)?

Determines the position and direction of a ray through the given point in the 2D space of the view.

**Required**

func unproject(CGPoint, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace, ontoPlane: float4x4) -> SIMD3&lt;Float>?

Unprojects a point from the view onto a plane in 3D world coordinates.

**Required**

## Relationships

### Conforming Types

- EntityTargetValue

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

- RealityViewCameraContent

## See Also

### Coordinate space conversions

protocol RealityCoordinateSpaceConverting

A value that can be converted between SwiftUI `CoordinateSpace` and RealityKit `Entity`.

struct SceneRealityCoordinateSpace

The coordinate space that represents the center of a RealityKit scene.

struct CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

protocol RealityCoordinateSpace

A 3D coordinate space that exists within a RealityKit hierarchy.

