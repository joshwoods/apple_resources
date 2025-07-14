

- Vision
-  Joint3D 

Structure

# Joint3D

An object that represents a body pose joint in 3D space.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Joint3D
```

## Topics

### Creating a joint

init(position: simd_float4x4, localPosition: simd_float4x4, identifer: String, parentJoint: String)

Creates a 3D joint.

### Inspecting a joint

let localPosition: simd_float4x4

The joint position relative to the parent joint.

let position: simd_float4x4

The joint position relative to the camera.

let parentJoint: String

The parent joint in the observation.

let identifier: String

The name of the joint.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### 3D body pose detection

class DetectHumanBodyPose3DRequest

A request that detects points on human bodies in 3D space, relative to the camera.

