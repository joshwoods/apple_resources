

- Vision
- VNDetectHumanHandPoseRequest
-  supportedJointNames 

Instance Property

# supportedJointNames

Retrieves the supported joint names.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
@nonobjc
var supportedJointNames: [VNHumanHandPoseObservation.JointName] { get throws }
```

## See Also

### Determining Supported Joints

class func supportedJointNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

var supportedJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

