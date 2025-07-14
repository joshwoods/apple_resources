

- RealityKit
-  MeshSkeletonCollection 

Structure

# MeshSkeletonCollection

An object that holds a collection of skeletons used by a mesh resource.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct MeshSkeletonCollection
```

## Topics

### Initializers

init()

init([MeshResource.Skeleton])

### Instance Properties

var count: Int

Number of skeletons.

var isEmpty: Bool

True if there are no skeletons.

### Instance Methods

func insert(MeshResource.Skeleton) -> Bool

Add a new skeleton to the container. Returns true if added.

func remove(id: String) -> MeshResource.Skeleton?

Remove a skeleton by id.

func removeAll()

Remove all the skeletons.

func update(MeshResource.Skeleton) -> MeshResource.Skeleton?

Update an existing skeleton. The old instance is returned.

### Subscripts

subscript(String) -> MeshResource.Skeleton?

Read a skeleton given its id.

### Default Implementations

Collection Implementations

ExpressibleByArrayLiteral Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- ExpressibleByArrayLiteral
- Sequence

## See Also

### Mesh skeletons

struct Skeleton

A skeleton consists of a hierarchy of joints. Each joint defines a coordinate space. Portions of a model may be thought of as having a position in a joint’s local space.

struct Joint

A named joint in a MeshResource.Skeleton.

typealias ID

A type representing the stable identity of the entity associated with an instance.

struct MeshJointInfluence

A binding to a joint, which consists of the joint’s index and the weight of that joint’s influence on a vertex.

struct JointInfluences

A buffer of vertex-joint influences which bind the mesh part’s vertices to a skeleton via a skinning deformation.

