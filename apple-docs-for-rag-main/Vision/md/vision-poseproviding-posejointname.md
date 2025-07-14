

- Vision
- PoseProviding
-  PoseJointName 

Associated Type

# PoseJointName

A type that represents a joint name.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
associatedtype PoseJointName : Decodable, Encodable, Hashable, RawRepresentable where Self.PoseJointName.RawValue == String
```

**Required**

## See Also

### Getting the joint names

var availableJointNames: [Self.PoseJointName]

The names of the available joints in the observation.

**Required**

