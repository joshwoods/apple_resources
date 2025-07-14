

- RealityKit
- MeshResource
-  MeshResource.JointInfluences 

Structure

# MeshResource.JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct JointInfluences
```

## Overview

Each vertex is associated with a fixed number of influences. If `influencesPerVertex` is 4, then there should be four elements in the buffer of joint influences for each vertex in the mesh part.

Note

If a particular vertex needs fewer influences than the `influencesPerVertex` value, the influences for that vertex can be padded with zero-weight influences.

## Topics

### Initializers

init(influences: MeshBuffers.JointInfluences, influencesPerVertex: Int)

Associates every vertex in the mesh with a fixed number of influences per vertex.

### Instance Properties

var influences: MeshBuffers.JointInfluences

Buffer of joint influences.

## See Also

### Mesh skeletons

struct Skeleton

A skeleton consists of a hierarchy of joints. Each joint defines a coordinate space. Portions of a model may be thought of as having a position in a joint’s local space.

struct Joint

A named joint in a MeshResource.Skeleton.

typealias ID

A type representing the stable identity of the entity associated with an instance.

struct MeshSkeletonCollection

An object that holds a collection of skeletons used by a mesh resource.

struct MeshJointInfluence

A binding to a joint, which consists of the joint’s index and the weight of that joint’s influence on a vertex.

