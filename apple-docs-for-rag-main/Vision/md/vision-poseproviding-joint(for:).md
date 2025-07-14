

- Vision
- PoseProviding
-  joint(for:) 

Instance Method

# joint(for:)

Retrieves a joint for a given joint name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func joint(for jointName: Self.PoseJointName) -> Joint?
```

**Required**

## See Also

### Getting the joints

func allJoints(in: Self.PoseJointsGroupName?) -> [Self.PoseJointName : Joint]

Retrieves a dictionary of all joints in the observation or joint group.

**Required**

