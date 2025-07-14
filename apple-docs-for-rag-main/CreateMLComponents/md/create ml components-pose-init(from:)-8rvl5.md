

- Create ML Components
- Pose
-  init(from:) 

Initializer

# init(from:)

Creates a pose from a dictionary of joint keypoints.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(from points: [JointKey : JointPoint])
```

## Parameters 

`points`  

A dictionary of pose joint keypoints, where keys are joint names and values are joint points.

## See Also

### Creating a pose

init(VNRecognizedPointsObservation) throws

Creates a pose from a body or hand pose observation.

