

- Vision
- VNDetectHumanBodyPoseRequest
-  supportedJointNames(forRevision:) Deprecated

Type Method

# supportedJointNames(forRevision:)

Retrieves the supported joint names for a revision.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func supportedJointNames(forRevision revision: Int) throws -> [VNHumanBodyPoseObservation.JointName]
```

## Parameters 

`revision`  

The body pose request revision.

## Return Value

The array of joint name objects for the specified revision.

## See Also

### Determining Supported Joints

var supportedJointNames: [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names.

var supportedJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

class func supportedJointsGroupNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names for a revision.

Deprecated

