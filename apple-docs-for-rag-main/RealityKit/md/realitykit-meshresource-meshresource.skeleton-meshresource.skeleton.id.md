

- RealityKit
- MeshResource
- MeshResource.Skeleton
-  MeshResource.Skeleton.ID 

Type Alias

# MeshResource.Skeleton.ID

A type representing the stable identity of the entity associated with an instance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
typealias ID = String
```

## See Also

### Mesh skeletons

struct Skeleton

A skeleton consists of a hierarchy of joints. Each joint defines a coordinate space. Portions of a model may be thought of as having a position in a joint’s local space.

struct Joint

A named joint in a MeshResource.Skeleton.

struct MeshSkeletonCollection

An object that holds a collection of skeletons used by a mesh resource.

struct MeshJointInfluence

A binding to a joint, which consists of the joint’s index and the weight of that joint’s influence on a vertex.

struct JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

