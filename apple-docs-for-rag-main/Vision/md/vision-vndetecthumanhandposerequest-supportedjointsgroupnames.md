

- Vision
- VNDetectHumanHandPoseRequest
-  supportedJointsGroupNames 

Instance Property

# supportedJointsGroupNames

Retrieves the supported joint group names.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
var supportedJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName] { get throws }
```

## See Also

### Determining Supported Joints

var supportedJointNames: [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

