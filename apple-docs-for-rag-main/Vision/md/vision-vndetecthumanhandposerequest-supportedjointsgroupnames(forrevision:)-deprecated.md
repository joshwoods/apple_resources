

- Vision
- VNDetectHumanHandPoseRequest
-  supportedJointsGroupNames(forRevision:) Deprecated

Type Method

# supportedJointsGroupNames(forRevision:)

Retrieves the supported joint group names for a revision.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func supportedJointsGroupNames(forRevision revision: Int) throws -> [VNHumanHandPoseObservation.JointsGroupName]
```

## Parameters 

`revision`  

The hand pose request revision.

## Return Value

The array of joint group name objects for the revision.

## See Also

### Determining Supported Joints

var supportedJointNames: [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanHandPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

var supportedJointsGroupNames: [VNHumanHandPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

