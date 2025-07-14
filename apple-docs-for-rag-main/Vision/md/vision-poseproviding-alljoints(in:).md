

- Vision
- PoseProviding
-  allJoints(in:) 

Instance Method

# allJoints(in:)

Retrieves a dictionary of all joints in the observation or joint group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func allJoints(in groupName: Self.PoseJointsGroupName?) -> [Self.PoseJointName : Joint]
```

**Required**

## Parameters 

`groupName`  

The group name to retrieve the joint names of.

## Return Value

The list of joints in the observation or joint group. If no `groupName` is specified, the system returns all joints in the observation..

## See Also

### Getting the joints

func joint(for: Self.PoseJointName) -> Joint?

Retrieves a joint for a given joint name.

**Required**

