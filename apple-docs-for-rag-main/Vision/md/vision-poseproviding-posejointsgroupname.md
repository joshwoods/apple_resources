

- Vision
- PoseProviding
-  PoseJointsGroupName 

Associated Type

# PoseJointsGroupName

A type that represents a joint group name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
associatedtype PoseJointsGroupName : CaseIterable, RawRepresentable where Self.PoseJointsGroupName.RawValue == String
```

**Required**

## See Also

### Getting the joint group names

var availableJointsGroupNames: [Self.PoseJointsGroupName]

The names of the available joint groupings in the observation.

**Required**

