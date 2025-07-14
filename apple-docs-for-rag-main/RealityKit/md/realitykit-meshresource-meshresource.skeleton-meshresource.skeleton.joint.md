

- RealityKit
- MeshResource
- MeshResource.Skeleton
-  MeshResource.Skeleton.Joint 

Structure

# MeshResource.Skeleton.Joint

A named joint in a MeshResource.Skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Joint
```

## Topics

### Operators

static func == (MeshResource.Skeleton.Joint, MeshResource.Skeleton.Joint) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(name: String, parentIndex: Int?, inverseBindPoseMatrix: simd_float4x4, restPoseTransform: Transform)

Creates a single joint in a skeleton.

### Instance Properties

var inverseBindPoseMatrix: simd_float4x4

A matrix which transforms from the authored pose (the “bind pose”) of the bound model to the local space of this joint.

var name: String

The name of this joint.

var parentIndex: Int?

The index of this joint’s parent, or nil if this joint has no parent.

var restPoseTransform: Transform

The local transform of this joint in skeleton’s rest pose, specified relative to this joint’s parent (or relative to model space, if this joint has no parent).

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Mesh skeletons

struct Skeleton

A skeleton consists of a hierarchy of joints. Each joint defines a coordinate space. Portions of a model may be thought of as having a position in a joint’s local space.

typealias ID

A type representing the stable identity of the entity associated with an instance.

struct MeshSkeletonCollection

An object that holds a collection of skeletons used by a mesh resource.

struct MeshJointInfluence

A binding to a joint, which consists of the joint’s index and the weight of that joint’s influence on a vertex.

struct JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

