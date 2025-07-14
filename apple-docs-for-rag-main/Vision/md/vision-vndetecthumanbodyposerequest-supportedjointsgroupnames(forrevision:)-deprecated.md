

- Vision
- VNDetectHumanBodyPoseRequest
-  supportedJointsGroupNames(forRevision:) Deprecated

Type Method

# supportedJointsGroupNames(forRevision:)

Retrieves the supported joint group names for a revision.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func supportedJointsGroupNames(forRevision revision: Int) throws -> [VNHumanBodyPoseObservation.JointsGroupName]
```

## Parameters 

`revision`  

The body pose request revision.

## Return Value

The array of joint group name objects for the revision.

## See Also

### Determining Supported Joints

var supportedJointNames: [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names.

class func supportedJointNames(forRevision: Int) throws -> [VNHumanBodyPoseObservation.JointName]

Retrieves the supported joint names for a revision.

Deprecated

var supportedJointsGroupNames: [VNHumanBodyPoseObservation.JointsGroupName]

Retrieves the supported joint group names.

