

- Vision
- VNDetectHumanBodyPoseRequest
-  supportedJointsGroupNames 

Instance Property

# supportedJointsGroupNames

Retrieves the supported joint group names.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
var supportedJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName] { get throws }
```

## See Also

### Determining Supported Joints

var supportedJointNames: [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

