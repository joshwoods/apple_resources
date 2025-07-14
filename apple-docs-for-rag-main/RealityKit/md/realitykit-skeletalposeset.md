

- RealityKit
-  SkeletalPoseSet 

Structure

# SkeletalPoseSet

A collection of named skeletal poses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SkeletalPoseSet
```

## Topics

### Initializers

init()

Creates an empty collection.

### Instance Properties

var count: Int

The number of elements in the collection.

var `default`: SkeletalPoseSet.Element?

Accesses the first skeletal pose.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

### Instance Methods

func contains(SkeletalPose.ID) -> Bool

Checks if the set contains a pose with the given name.

func index(of: SkeletalPose.ID) -> SkeletalPoseSet.Index?

Returns the index where the specified pose appears in the collection.

func set(SkeletalPoseSet.Element) -> SkeletalPoseSet.Element?

Updates a pose in the set based on its name. If pose with this ID does not exist, does nothing.

### Subscripts

subscript(SkeletalPose.ID) -> SkeletalPoseSet.Element?

Accesses the element with the specified identifier.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Copyable
- Sequence

## See Also

### Skeletons

struct SkeletalPosesComponent

A component that exposes the collection of named animation skeletal poses.

struct SkeletalPose

A container that holds the position and orientation of each joint in a single animation skeleton.

typealias ID

A type representing the stable identity of the entity associated with an instance.

typealias Element

A type representing the sequence’s elements.

