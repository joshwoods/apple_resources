

- Vision
- HumanBodyPose3DObservation
-  allJoints(in:) 

Instance Method

# allJoints(in:)

Retrieves a dictionary of all joints in a joint group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func allJoints(in groupName: HumanBodyPose3DObservation.JointsGroupName? = nil) -> [HumanBodyPose3DObservation.JointName : Joint3D]
```

## See Also

### Getting the joints

var availableJointsGroupNames: [HumanBodyPose3DObservation.JointsGroupName]

The names of the available joint groupings in the observation.

enum JointsGroupName

The supported joint group names for the body pose.

func joint(for: HumanBodyPose3DObservation.JointName) -> Joint3D?

Retrieves a joint for a given joint name.

var availableJointNames: [HumanBodyPose3DObservation.JointName]

The names of the available joints in the observation.

enum JointName

The supported joint names for the body pose.

