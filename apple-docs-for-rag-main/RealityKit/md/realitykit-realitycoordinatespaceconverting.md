

- RealityKit
-  RealityCoordinateSpaceConverting 

Protocol

# RealityCoordinateSpaceConverting

A value that can be converted between SwiftUI `CoordinateSpace` and RealityKit `Entity`.

RealityKitSwiftUIvisionOS 1.0+

``` source
protocol RealityCoordinateSpaceConverting
```

## Topics

### Instance Methods

func convert(Rotation3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> simd_quatf

Converts a Rotation3D from a defined SwiftUI coordinate space to a quaternion in a RealityKit coordinate space.

func convert(Rect3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> BoundingBox

Converts a Rect3D from a defined SwiftUI coordinate space to a BoundingBox in a RealityKit coordinate space.

func convert(AffineTransform3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> Transform

Returns a 3D Transform converted from a defined SwiftUI coordinate space to a RealityKit coordinate space.

func convert(Size3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> SIMD3&lt;Float>

Converts a Size3D from a defined SwiftUI coordinate space to a 3D size vector in a RealityKit coordinate space.

func convert(Vector3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> SIMD3&lt;Float>

ConvConverts a 3D vector from a SwiftUI coordinate space to one in a RealityKit coordinate space.

func convert(Point3D, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> SIMD3&lt;Float>

Converts a `Point3D` from a defined SwiftUI coordinate space to a 3D point in a RealityKit coordinate space.

func convert(boundingBox: BoundingBox, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> Rect3D

Converts a BoundingBox from a RealityKit coordinate space to a Rect3D in a defined SwiftUI coordinate space.

func convert(point: SIMD3&lt;Float>, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> Point3D

Converts a 3D point from a RealityKit coordinate space to one in a SwiftUI coordinate space.

func convert(rotation: simd_quatf, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> Rotation3D

Converts a quaternion from a RealityKit coordinate space to a Rotation3D in a defined SwiftUI coordinate space.

func convert(size: SIMD3&lt;Float>, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> Size3D

Converts a 3D size vector from a RealityKit coordinate space to a Size3D in a defined SwiftUI coordinate space.

func convert(transform: Transform, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> AffineTransform3D

Returns an AffineTransform3D converted from a RealityKit coordinate space to a defined SwiftUI coordinate space.

func convert(vector: SIMD3&lt;Float>, from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> Vector3D

Converts a 3D vector from a RealityKit coordinate space to one in a SwiftUI coordinate space.

func transform(from: some RealityCoordinateSpace, to: some CoordinateSpaceProtocol) -> AffineTransform3D

**Required**

func transform(from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> AffineTransform3D

**Required**

## Relationships

### Conforming Types

- EntityTargetValue

  Conforms when `Value` conforms to `Copyable` and `Escapable`.

- RealityViewContent

## See Also

### Coordinate space conversions

struct SceneRealityCoordinateSpace

The coordinate space that represents the center of a RealityKit scene.

struct CameraRealityCoordinateSpace

The coordinate space that represents the scene’s active camera.

protocol RealityCoordinateSpace

A 3D coordinate space that exists within a RealityKit hierarchy.

protocol RealityCoordinateSpaceProjecting

A protocol for coordinate spaces that can project 2D points to and from 3D.

