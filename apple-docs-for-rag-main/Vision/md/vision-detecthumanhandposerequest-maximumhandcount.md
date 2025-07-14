

- Vision
- DetectHumanHandPoseRequest
-  maximumHandCount 

Instance Property

# maximumHandCount

The maximum number of hands to detect in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var maximumHandCount: Int
```

## Discussion

The request orders detected hands by relative size, with only the largest ones having key points determined.

The default value is `2`.

## See Also

### Inspecting a request

var supportedJointNames: [HumanHandPoseObservation.JointName]

The joint names the request supports.

var supportedJointsGroupNames: [HumanHandPoseObservation.JointsGroupName]

The joint group names the request supports.

