

- RealityKit
-  MeshJointInfluence 

Structure

# MeshJointInfluence

A binding to a joint, which consists of the joint’s index and the weight of that joint’s influence on a vertex.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct MeshJointInfluence
```

## Overview

A vertex may be influenced by one or more joints. The skinned position of that vertex is defined by a set of MeshJointInfluence values whose weights sum to 1. The skinned position is given by:

```
position = vertexPosition(transformedByJoint: influences[0].jointIndex) * influences[0].weight
         + vertexPosition(transformedByJoint: influences[1].jointIndex) * influences[1].weight
         + ...
```

The skinned position of a vertex is a linear combination of the vertex’s position transformed by each joint, with weights given by the MeshJointInfluence values.

To transform a vertex position by a joint, the initial vertex position is first transformed by the joint’s inverse bind pose matrix, then by the local-to-parent transform of the joint, and finally by the local-to-parent transform of each of the joint’s parents.

## Topics

### Initializers

init()

init(jointIndex: Int, weight: Float)

### Instance Properties

var jointIndex: Int

var weight: Float

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

struct JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

