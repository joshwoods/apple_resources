

- Vision
- DetectHumanBodyPoseRequest
-  detectsHands 

Instance Property

# detectsHands

A Boolean value that detects hands of the body in the results, if they’re visible.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var detectsHands: Bool
```

## Discussion

The default value is `true,` and requires DetectHumanBodyPoseRequest.Revision.revision2.

## See Also

### Inspecting a request

var supportedJointNames: [HumanBodyPoseObservation.JointName]

The joint names the request supports.

var supportedJointsGroupNames: [HumanBodyPoseObservation.JointsGroupName]

The joint group names the request supports.

