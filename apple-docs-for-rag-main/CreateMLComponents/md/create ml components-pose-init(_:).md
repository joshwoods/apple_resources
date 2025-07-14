

- Create ML Components
- Pose
-  init(\_:) 

Initializer

# init(\_:)

Creates a pose from a body or hand pose observation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(_ observation: VNRecognizedPointsObservation) throws
```

## Parameters 

`observation`  

Recognized points observation that comes from either a body pose or hand pose request.

## See Also

### Creating a pose

init(from: [JointKey : JointPoint])

Creates a pose from a dictionary of joint keypoints.

