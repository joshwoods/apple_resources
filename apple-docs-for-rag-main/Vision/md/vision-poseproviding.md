

- Vision
-  PoseProviding 

Protocol

# PoseProviding

An observation that provides a collection of joints that make up a pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol PoseProviding
```

## Topics

### Getting the joints

func joint(for: Self.PoseJointName) -> Joint?

Retrieves a joint for a given joint name.

**Required**

func allJoints(in: Self.PoseJointsGroupName?) -> [Self.PoseJointName : Joint]

Retrieves a dictionary of all joints in the observation or joint group.

**Required**

### Getting the joint names

var availableJointNames: [Self.PoseJointName]

The names of the available joints in the observation.

**Required**

associatedtype PoseJointName : Decodable, Encodable, Hashable, RawRepresentable

A type that represents a joint name.

**Required**

### Getting the joint group names

var availableJointsGroupNames: [Self.PoseJointsGroupName]

The names of the available joint groupings in the observation.

**Required**

associatedtype PoseJointsGroupName : CaseIterable, RawRepresentable

A type that represents a joint group name.

**Required**

## Relationships

### Conforming Types

- AnimalBodyPoseObservation
- HumanBodyPoseObservation
- HumanHandPoseObservation

## See Also

### Body and hand pose detection

struct DetectHumanBodyPoseRequest

A request that detects a human body pose.

struct DetectHumanHandPoseRequest

A request that detects a human hand pose.

enum Chirality

The hand sidedness of a pose.

struct Joint

A pose joint represented as a normalized point in an image, along with a label and a confidence value.

